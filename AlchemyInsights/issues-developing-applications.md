---
title: ปัญหาในการพัฒนาแอปพลิเคชัน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013443"
---
# <a name="issues-developing-applications"></a>ปัญหาในการพัฒนาแอปพลิเคชัน

เมื่อต้องการแก้ไขปัญหาที่พบบ่อยที่สุดเมื่อสร้างAzure Active Directoryแอป (AD) ให้ดูบทความต่อไปนี้:

- [ฉันเห็นปัญหาในการลงชื่อเข้าใช้แอปพลิเคชันโดยใช้เบราว์เซอร์ Chrome เท่านั้น](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [ฉันไม่ทราบวิธีการเปลี่ยนค่าเริ่มต้นอายุการใช้งานโทเค็นของแอปพลิเคชันของฉัน](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [ฉันสับสนเกี่ยวกับวิธีการรับความยินยอมจากแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [ฉันไม่ทราบวิธีการให้สิทธิ์กับแอปพลิเคชันของฉัน](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [ฉันไม่เข้าใจความแตกต่างระหว่างสิทธิ์ของแอปพลิเคชันที่ได้รับมอบสิทธิ์](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***การสิ้นสุดการสนับสนุนAzure Active Directory (ADAL) และ Azure AD Graph API (AAD Graph)***

- ตั้งแต่วันที่ 30 มิถุนายน 2020 เราจะไม่เพิ่มฟีเจอร์ใหม่ใดๆ ลงใน Azure Active Directory Authentication Library (ADAL) และ Azure AD Graph API (AAD Graph) อีกต่อไป เราจะให้การสนับสนุนด้านเทคนิคและการอัปเดตความปลอดภัยต่อไป แต่จะไม่มีการอัปเดตฟีเจอร์อีกต่อไป

- ตั้งแต่วันที่ 30 มิถุนายน 2022 เราจะสิ้นสุดการสนับสนุน ADAL และ AAD Graph และจะไม่มีการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยอีกต่อไป เนื่องจากเงื่อนไขนี้ สิ่งต่อไปนี้เป็นผลกระทบ:

    - แอปที่ใช้ ADAL บนเวอร์ชัน OS ที่มีอยู่จะยังคงสามารถใช้งานต่อหลังจากนี้ แต่จะไม่รับการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยใดๆ

    - แอปที่ใช้ AAD Graphหลังจากนี้อาจไม่ได้รับการตอบกลับจากจุดสิ้นสุด AAD Graphอีกต่อไป

**การโยกย้าย ADAL**

ถ้าคุณใช้งานแอปของ Microsoft เราขอแนะนนะให้อัปเดตเป็น ไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL) ซึ่งมีฟีเจอร์ล่าสุดและการอัปเดตความปลอดภัย ข้อแนะน้นี้อยู่ในบริบทของ Microsoft ที่เริ่มต้นกระบวนการโยกย้ายแอปไปยัง MSAL ภายในวันที่สิ้นสุดการสนับสนุน 

การโยกย้ายโดย Microsoft ของแอปไปยัง MSAL จะรับรองว่าแอปได้รับประโยชน์จากการปรับปรุงความปลอดภัยและฟีเจอร์ที่ต่อเนื่องของ MSAL

1. [อ่าน ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [เรียนรู้เกี่ยวกับวิธีการโยกย้ายแอปตามแพลตฟอร์ม](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. ถ้าคุณต้องการความช่วยเหลือในการเข้าใจว่าแอปใดของคุณใช้ ADAL เราขอแนะนนะให้คุณตรวจสอบโค้ดต้นฉบับของแอปทั้งหมด และถ้าสามารถติดต่อผู้ออกซอฟต์แวร์อิสระ (ISVs) หรือผู้ให้บริการแอปรายใดก็ได้ ฝ่ายสนับสนุนของ Microsoft ยังสามารถแสดงรายการแอปที่ไม่ใช่ Microsoft ADAL ทั้งหมดในผู้เช่าของคุณ

**การโยกย้าย AAD Graph**

สําหรับแอปพลิเคชันที่ใช้ AAD Graph ให้ปฏิบัติตามแนวทางของเราเพื่อโยกย้าย AAD Graphแอปไปยัง Microsoft Graph:

1. [รายการตรวจสอบการโยกย้ายของเราให้จุดเริ่มต้น](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
2. พอร์ทัลการลงทะเบียนแอป Azure ของคุณจะแสดงแอปพลิเคชันที่ใช้ AAD Graph เราขอแนะนนะให้คุณตรวจสอบโค้ดต้นฉบับของแอปของคุณทั้งหมด และถ้าสามารถติดต่อผู้ขายซอฟต์แวร์อิสระ (ISVs) หรือผู้ให้บริการแอปรายใดก็ได้ ฝ่ายสนับสนุนของ Microsoft ยังสามารถให้ข้อมูลเกี่ยวกับการใช้งาน AAD Graphในผู้เช่าของคุณ







