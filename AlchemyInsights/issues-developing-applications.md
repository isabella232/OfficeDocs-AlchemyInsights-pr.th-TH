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
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974765"
---
# <a name="issues-developing-applications"></a>ปัญหาในการพัฒนาแอปพลิเคชัน

เมื่อต้องการแก้ไขปัญหาทั่วไปที่พบมากที่สุดเมื่อสร้างแอป Azure Active Directory (AD) ให้ดูบทความต่อไปนี้:

- [ฉันเห็นปัญหาในการลงชื่อเข้าใช้แอปพลิเคชันโดยใช้เบราว์เซอร์ Chrome เท่านั้น](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [ฉันไม่ทราบวิธีการเปลี่ยนค่าเริ่มต้นตลอดอายุการใช้งานของโทเค็นสำหรับแอปพลิเคชันของฉัน](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [ฉันสับสนเกี่ยวกับวิธีการทำงานของความยินยอมของแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [ฉันไม่ทราบวิธีการให้สิทธิ์กับแอปพลิเคชันของฉัน](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [ฉันไม่เข้าใจความแตกต่างระหว่างสิทธิ์ที่มอบหมายและแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***จุดสิ้นสุดของการสนับสนุนสำหรับ Azure Active Directory ไลบรารีการรับรองความถูกต้อง (ADAL) และ AZURE AD graph (graph)** _

- เริ่มต้นวันที่30มิถุนายน๒๐๒๐เราจะไม่เพิ่มฟีเจอร์ใหม่อีกต่อไปในไลบรารีการรับรองความถูกต้องของ Azure Active Directory (ADAL) และ Azure AD Graph (Graph Graph) เราจะยังคงให้การสนับสนุนทางเทคนิคและการอัปเดตความปลอดภัยแต่จะไม่มีการอัปเดตของฟีเจอร์อีกต่อไป

- เริ่มต้นวันที่30มิถุนายน๒๐๒๒เราจะสิ้นสุดการสนับสนุนสำหรับ ADAL และ AAD กราฟและจะไม่ให้การสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยอีกต่อไป ผลลัพธ์ของเงื่อนไขนี้จะมีผลกระทบต่อไปนี้:

    - แอปที่ใช้ ADAL บน OS เวอร์ชันที่มีอยู่จะยังคงทำงานต่อไปหลังจากเวลานี้แต่จะไม่ได้รับการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัย

    - แอปที่ใช้กราฟ AAD หลังจากเวลานี้อาจไม่ได้รับการตอบสนองจากจุดสิ้นสุดของกราฟ AAD

การ *โยกย้าย _ ADAL**

ถ้าคุณกำลังใช้แอป Microsoft เราขอแนะนำให้อัปเดตเป็นไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL) ซึ่งมีฟีเจอร์และการอัปเดตความปลอดภัยล่าสุด คำแนะนำนี้อยู่ในบริบทของ Microsoft ในการเริ่มต้นกระบวนการโยกย้ายแอปของแอปไปยัง MSAL โดยกำหนดเวลาสิ้นสุดของการสนับสนุน 

การโยกย้ายโดยไมโครซอฟท์ของแอ MSAL เพื่อให้แน่ใจว่าแอปจะได้รับประโยชน์จากการปรับปรุงความปลอดภัยและฟีเจอร์ที่ต่อเนื่องของ MSAL

1. [อ่านคำถามที่ถามบ่อยเกี่ยวกับ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [เรียนรู้เกี่ยวกับวิธีการโยกย้ายแอปบนไซต์ต่อเนื่อง](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. ถ้าคุณต้องการความช่วยเหลือในการทำความเข้าใจที่แอปของคุณใช้ ADAL เราขอแนะนำให้คุณตรวจทานโค้ดต้นฉบับของแอพทั้งหมดของคุณและถ้ามีให้ติดต่อผู้จำหน่ายซอฟต์แวร์อิสระ (Isv) หรือผู้ให้บริการแอป ฝ่ายสนับสนุนของ microsoft ยังสามารถให้คุณมีรายการของแอป ADAL ที่ไม่ใช่ Microsoft ทั้งหมดในผู้เช่าของคุณ

**การโยกย้ายกราฟ AAD**

สำหรับแอปพลิเคชันที่ใช้กราฟ AAD ให้ทำตามคำแนะนำของเราในการโยกย้ายแอปการใช้กราฟ AAD ไปยัง Microsoft Graph:

1. [รายการตรวจสอบการโยกย้ายของเรามีจุดเริ่มต้นใช้](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)งาน 
2. พอร์ทัลการลงทะเบียนแอ Azure ของคุณแสดงแอปพลิเคชันที่ใช้กราฟ AAD เราขอแนะนำให้คุณตรวจทานโค้ดต้นฉบับของแอปของคุณทั้งหมดและถ้ามีผลบังคับให้ติดต่อผู้จำหน่ายซอฟต์แวร์อิสระ (Isv) หรือผู้ให้บริการแอป ฝ่ายสนับสนุนของ Microsoft ยังสามารถให้ข้อมูลเกี่ยวกับการใช้งานของการใช้กราฟ AAD ในผู้เช่าของคุณได้อีกด้วย







