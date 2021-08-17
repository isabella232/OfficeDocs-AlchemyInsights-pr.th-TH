---
title: แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) แบบ OIDC
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
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105803"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) แบบ OIDC

- เมื่อต้องการเรียนรู้วิธีการเพิ่มแอป OIDC ไปยังผู้เช่า Azure ของคุณ ให้ดู คู่มือเริ่มต้นใช้งานด่วน: ตั้งค่าการลงชื่อเข้าระบบครั้งเดียว[(SSO) แบบ OIDC ให้กับ](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)แอปพลิเคชันในผู้เช่า Azure Active Directory (Azure AD) ของคุณ
- For more details about apps that use the OpenID เชื่อมต่อ standard to implement single sign-on, [see Understand OIDC-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- For information in case you choose to write your code by directly sending and handling HTTP requests or use a third-party open-source library, than using one of our open-source libraries, see [OAuth 2.0 and OpenID เชื่อมต่อ protocols on the แพลตฟอร์มข้อมูลประจําตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**โพรโทคอล**

1. [แพลตฟอร์มข้อมูลประจําตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)และโฟลว์การให้สิทธิ์โดยนัย - คุณลักษณะการมอบหมายโดยนัยคือ โทเค็น (โทเค็น ID หรือโทเค็นการเข้าถึง) จะถูกส่งกลับโดยตรงจากจุดสิ้นสุด /authorize แทนจุดสิ้นสุด /token ซึ่งมักจะถูกใช้เป็นส่วนหนึ่งของโฟลว์รหัสการรับรองความถูกต้อง ในสิ่งที่เรียกว่า "โฟลว์แบบไฮบริด" - การเรียกโทเค็น ID บน **การร้องขอ /authorize พร้อมกับรหัส** การตรวจสอบ บทความนี้จะอธิบายวิธีการเขียนโปรแกรมโดยตรงกับโพรโทคอลในแอปพลิเคชันของคุณเพื่อขอโทเค็นจาก Azure AD
2. แพลตฟอร์มข้อมูลประจําตัวของ Microsoft การอนุญาต[OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - การอนุญาตรหัส OAuth 2.0 สามารถใช้ในแอปที่ติดตั้งบนอุปกรณ์เพื่อให้สามารถเข้าถึงทรัพยากรที่ได้รับการป้องกัน เช่น API เว็บ ด้วยการใช้แพลตฟอร์มข้อมูลประจําตัวของ Microsoft OAuth 2.0 คุณสามารถเพิ่ม **การลงชื่อเข้าใช้และการเข้าถึง API ไปยังแอปบนอุปกรณ์เคลื่อนที่และเดสก์ท็อป** ของคุณ บทความนี้จะอธิบายวิธีการเขียนโปรแกรมโดยตรงกับโพรโทคอลในแอปพลิเคชันของคุณโดยใช้ภาษาใดก็ได้
3. [แพลตฟอร์มข้อมูลประจําตัวของ Microsoft OpenID เชื่อมต่อ](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc)- เมื่อคุณใช้การปรับใช้ OpenID เชื่อมต่อ ของ แพลตฟอร์มข้อมูลประจําตัวของ Microsoft คุณสามารถเพิ่มการเข้าถึงการลงชื่อเข้าใช้และ API ไปยังแอปของคุณ บทความนี้แสดงวิธีการแยกภาษาและอธิบายวิธีการส่งและรับข้อความ HTTP **โดยไม่ใช้ไลบรารีโอเพนซอร์สใดๆ ของ Microsoft**
4. แพลตฟอร์มข้อมูลประจําตัวของ Microsoft โฟลว์ข้อมูลเฉพาะตัวของไคลเอ็นต์ [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - คุณสามารถใช้ข้อมูลรับรองความถูกต้องของไคลเอ็นต์ OAuth 2.0 ที่ระบุใน RFC 6749 ซึ่งบางครั้งเรียกว่า **OAuth** แบบสองทางเพื่อเข้าถึงทรัพยากรที่โฮสต์เว็บโดยใช้ข้อมูลเฉพาะตัวของแอปพลิเคชัน โดยทั่วไปแล้ว สิทธิ์ชนิดนี้จะใช้กับการโต้ตอบระหว่างเซิร์ฟเวอร์ถึงเซิร์ฟเวอร์ที่ต้องเรียกใช้ในเบื้องหลัง โดยไม่มีการโต้ตอบแบบทันทีกับผู้ใช้ แอปพลิเคชันประเภทนี้มักเรียกว่า **daemon หรือ****บัญชีบริการ** บทความนี้จะอธิบายวิธีการเขียนโปรแกรมโดยตรงกับโพรโทคอลในแอปพลิเคชันของคุณ
