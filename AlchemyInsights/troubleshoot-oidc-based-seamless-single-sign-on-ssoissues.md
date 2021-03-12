---
title: แก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่น (SSO) โดยใช้ OIDC
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747133"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>แก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่น (SSO) โดยใช้ OIDC

- เมื่อต้องการเรียนรู้วิธีการเพิ่มแอป OIDC ไปยังผู้เช่า Azure ของคุณ ให้ดูการเริ่มต้นใช้งานด่วน: ตั้งค่าการลงชื่อเข้าระบบครั้งเดียว [(SSO) แบบ OIDC](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)ให้กับแอปพลิเคชันในผู้เช่า Azure Active Directory (Azure AD) ของคุณ
- For more details about apps that use the OpenID Connect standard to implement single sign-on, [see Understand OIDC-based single sign-on.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- For information in case you choose to write your code by directly send and handling http requests or use a third-party open-source library, rather using one of our open-source libraries, see [OAuth 2.0 and OpenID Connect protocols on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**โพรโทคอล**

1. [แพลตฟอร์ม](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) ข้อมูลเฉพาะตัวของไมโครซอฟท์และขั้นตอนการให้สิทธิ์โดยนัย - ลักษณะการมอบหมายโดยนัยคือ โทเค็น (โทเค็น ID หรือโทเค็นการเข้าถึง) จะถูกส่งกลับโดยตรงจากจุดสิ้นสุด /authorize แทนจุดสิ้นสุด /token ซึ่งมักจะถูกใช้เป็นส่วนหนึ่งของโฟลว์รหัสการตรวจสอบ ในที่เรียกว่า "โฟลว์แบบไฮบริด" - การเรียกโทเค็น ID บน **การร้องขอ /authorize พร้อมกับรหัสการตรวจสอบ** บทความนี้จะอธิบายวิธีการเขียนโปรแกรมโดยตรงกับโพรโทคอลในแอปพลิเคชันของคุณเพื่อขอโทเค็นจาก Azure AD
2. แพลตฟอร์มข้อมูลเฉพาะตัวของไมโครซอฟท์และโฟลว์รหัสการรับรองความถูกต้อง[OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - การอนุญาตรหัส OAuth 2.0 สามารถใช้ในแอปที่ติดตั้งบนอุปกรณ์เพื่อเข้าถึงทรัพยากรที่มีการป้องกัน เช่น API เว็บ คุณสามารถเพิ่มการลงชื่อเข้าใช้และการเข้าถึง **API** ไปยังแอปบนอุปกรณ์เคลื่อนที่และเดสก์ท็อปของคุณโดยใช้การปรับใช้แพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft ของ OAuth 2.0 บทความนี้จะอธิบายวิธีการเขียนโปรแกรมโดยตรงกับโพรโทคอลในแอปพลิเคชันของคุณโดยใช้ภาษาใดก็ได้
3. [แพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft และโพรโทคอล OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - เมื่อคุณใช้การปรับใช้แพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft OpenID Connect คุณสามารถเพิ่มการลงชื่อเข้าใช้และการเข้าถึง API ไปยังแอปของคุณ บทความนี้แสดงวิธีแยกภาษาและอธิบายวิธีการส่งและรับข้อความ HTTP **โดยไม่ต้องใช้ไลบรารีโอเพนซอร์** สของ Microsoft
4. แพลตฟอร์มข้อมูลเฉพาะตัวของไมโครซอฟท์และโฟลว์ข้อมูลเฉพาะตัวของไคลเอ็นต์ [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - คุณสามารถใช้การอนุญาตให้ข้อมูลเฉพาะตัวของไคลเอ็นต์ OAuth 2.0 ที่ระบุใน RFC 6749 ซึ่งบางครั้งเรียกว่า **OAuth** แบบสองทางเพื่อเข้าถึงทรัพยากรที่โฮสต์บนเว็บโดยใช้ข้อมูลเฉพาะตัวของแอปพลิเคชัน โดยทั่วไปแล้วสิทธิ์ชนิดนี้จะใช้กับการโต้ตอบระหว่างเซิร์ฟเวอร์ถึงเซิร์ฟเวอร์ที่ต้องเรียกใช้ในเบื้องหลัง โดยไม่มีการโต้ตอบกับผู้ใช้ในทันที แอปพลิเคชันประเภทนี้มักจะเรียกว่า **daemon หรือ****บัญชี** บริการ บทความนี้จะอธิบายวิธีการเขียนโปรแกรมกับโพรโทคอลในแอปพลิเคชันของคุณโดยตรง
