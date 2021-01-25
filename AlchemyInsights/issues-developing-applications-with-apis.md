---
title: ปัญหาในการพัฒนาแอปพลิเคชันด้วย APIs
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975020"
---
# <a name="issues-developing-applications-with-apis"></a>ปัญหาในการพัฒนาแอปพลิเคชันด้วย APIs

เมื่อต้องการเริ่มต้นใช้งาน API กราฟของ Active Directory ของ Azure ให้ดูที่คู่มือการอ้างอิงของ azure [Ad graph quickstart](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) หรือดู [เอกสารอ้างอิงการอ้างอิง API ของ azure ad](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)ของ azure แบบโต้ตอบ

**การสิ้นสุดการสนับสนุนสำหรับ Azure Active Directory ไลบรารีการรับรองความถูกต้อง (ADAL) และ Azure AD Graph (Graph Graph)**

**เริ่มต้นวันที่30มิถุนายน๒๐๒๐** เราจะไม่เพิ่มฟีเจอร์ใหม่ให้กับกราฟ ADAL และ Azure AD อีกต่อไป เราจะยังคงให้การสนับสนุนทางเทคนิคและการอัปเดตความปลอดภัยแต่จะไม่มีการอัปเดตของฟีเจอร์อีกต่อไป

**เริ่มต้นวันที่30มิถุนายน๒๐๒๒** เราจะสิ้นสุดการสนับสนุนสำหรับ ADAL และ Azure AD Graph และจะไม่มีการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยอีกต่อไป

แอปที่ใช้ ADAL บน OS เวอร์ชันที่มีอยู่จะยังคงทำงานต่อไปหลังจากเวลานี้แต่จะไม่ได้รับการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัย

แอปที่ใช้กราฟโฆษณา Azure หลังจากเวลานี้อาจไม่ได้รับการตอบกลับจากจุดสิ้นสุดของกราฟ AD Azure อีกต่อไป

**การโยกย้าย ADAL**

เราขอแนะนำให้อัปเดตเป็น [ไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)ซึ่งมีฟีเจอร์และการอัปเดตความปลอดภัยล่าสุด

ถ้าคุณกำลังใช้แอป Microsoft ให้ทราบว่า Microsoft อยู่ในระหว่างการโยกย้ายแอปพลิเคชันของแอปพลิเคชันไปยัง MSAL ตามกำหนดเวลาสิ้นสุดของการสนับสนุนเพื่อให้แน่ใจว่าพวกเขาจะได้รับประโยชน์จากการปรับปรุงความปลอดภัยและฟีเจอร์ที่ต่อเนื่องของ MSAL

1. [อ่านคำถามที่ถามบ่อยเกี่ยวกับ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [เรียนรู้เกี่ยวกับวิธีการโยกย้ายแอปบนไซต์สำหรับแต่ละแพลตฟอร์ม](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. ถ้าคุณต้องการความช่วยเหลือในการทำความเข้าใจเกี่ยวกับแอปที่คุณใช้ ADAL เราขอแนะนำให้คุณตรวจทานโค้ดต้นฉบับของแอพทั้งหมดของคุณและถ้ามีให้เข้าถึง Isv หรือผู้ให้บริการแอป ฝ่ายสนับสนุนของ microsoft ยังสามารถให้คุณมีรายการของแอป ADAL ที่ไม่ใช่ Microsoft ทั้งหมดในผู้เช่าของคุณ

**การโยกย้ายกราฟ AAD**

สำหรับแอปพลิเคชันที่ใช้กราฟโฆษณา Azure ให้ทำตามคำแนะนำของเราในการโยกย้าย[แอป AZURE AD graph ไปยัง Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [รายการตรวจสอบการโยกย้ายของเรามีจุดเริ่มต้นใช้](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)งาน 
1. พอร์ทัลการลงทะเบียนแอ Azure ของคุณแสดงแอปพลิเคชันที่ใช้กราฟ AAD เราขอแนะนำให้คุณตรวจทานโค้ดต้นฉบับของแอปของคุณทั้งหมดและถ้ามีผลบังคับให้ติดต่อกับ Isv หรือผู้ให้บริการแอป ฝ่ายสนับสนุนของ Microsoft ยังสามารถให้คุณมีรายการของการใช้งานการใช้กราฟ AAD ทั้งหมดในผู้เช่าของคุณ
1. สำหรับแอปของคุณเพื่อเข้าถึงข้อมูลใน Microsoft Graph ผู้ใช้หรือผู้ดูแลระบบต้องให้สิทธิ์ที่ถูกต้องผ่านทางกระบวนการยินยอม การ [อ้างอิงสิทธิ์ของ Microsoft graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) จะแสดงรายการสิทธิ์ที่เกี่ยวข้องกับชุดหลักของ Microsoft graph APIs แต่ละชุด นอกจากนี้ยังมีคำแนะนำเกี่ยวกับวิธีการใช้สิทธิ์
