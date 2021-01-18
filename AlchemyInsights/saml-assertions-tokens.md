---
title: การยืนยันของ SAML (โทเค็น)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885678"
---
# <a name="saml-assertions-tokens"></a>การยืนยันของ SAML (โทเค็น)

1. โทเค็นภาษามาร์กอัปสิทธิ์การใช้งานของการรับรองความปลอดภัย (SAML) คือ XML ที่ใช้ในการอ้างสิทธิ์ ตามค่าเริ่มต้นโทเค็น SAML ของ Windows ตสื่อสารมูลฐาน (WCF) ใช้ในสถานการณ์การรักษาความปลอดภัยที่ติดต่อกับภายนอกโทเค็นที่ออก สำหรับข้อมูลเพิ่มเติมให้ดูที่[โทเค็นของ SAML และการอ้างสิทธิ์](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. แพลตฟอร์มสำหรับข้อมูลเฉพาะตัวของ Microsoft จะปล่อยโทเค็นความปลอดภัยหลายชนิดในการประมวลผลการรับรองความถูกต้องของแต่ละขั้นตอน การ[อ้างอิงการอ้างสิทธิ์โทเค็น saml](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)จะอธิบายรูปแบบลักษณะความปลอดภัยและเนื้อหาของโทเค็น๒.๐ของ saml
3. ทำตามคำแนะนำในการกำหนดค่าของโทเค็นที่สามารถกำหนดค่าได้ [ใน Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) เพื่อทำความเข้าใจวิธีการกำหนดค่าอายุการใช้งานของโทเค็น
4. ทำตามขั้นตอนที่ระบุไว้ใน [บทความนี้](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) เพื่อทำความเข้าใจเกี่ยวกับวิธีการกำหนดค่าการเข้ารหัสลับโทเค็นการ SAML AD ของ Azure
5. ใน Azure AD คุณสามารถตั้งค่าตัวเลือกการเซ็นชื่อใบรับรองและอัลกอริทึมการเซ็นชื่อใบรับรองได้ สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ตัวเลือกการเซ็นชื่อใบรับรองขั้นสูงในโทเค็น SAML สำหรับแอปแกลเลอรีใน Azure Active directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)
