---
title: ปัญหาเกี่ยวกับไลบรารีการรับรองความถูกต้อง
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028023"
---
# <a name="issues-with-authentication-libraries"></a>ปัญหาเกี่ยวกับไลบรารีการรับรองความถูกต้อง

1. [แพลตฟอร์มข้อมูลประจําตัวของ Microsoftไลบรารีการรับรองความถูกต้อง](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)รายการไลบรารีไคลเอ็นต์และไลบรารี middleware ที่ได้รับการสนับสนุนจาก Microsoft และที่เข้ากันได้
2. ไลบรารี Microsoft Authentication Library (MSAL) สนับสนุน [โฟลว์การรับรองความถูกต้อง](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) หลายอย่างเพื่อใช้ในสถานการณ์ของแอปพลิเคชันต่างๆ
3. เมื่อต้องการรับรองความถูกต้องและรับโทเค็น ให้คุณเตรียมใช้งานแอปพลิเคชันไคลเอ็นต์สาธารณะหรือแอปพลิเคชันที่เป็นความลับใหม่ในโค้ดของคุณ คุณสามารถตั้งค่าตัวเลือกการกําหนดค่าได้หลายตัวเลือกเมื่อคุณเตรียมใช้งานแอปไคลเอ็นต์ในไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL) เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู [ตัวเลือกการกําหนดค่า](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)แอปพลิเคชัน

**การสิ้นสุดการสนับสนุนAzure Active Directory (ADAL) และ Azure AD Graph API (AAD Graph)**

**ตั้งแต่วันที่ 30 มิถุนายน 2020** เราจะไม่เพิ่มฟีเจอร์ใหม่ใดๆ ลงใน ADAL และ Azure AD Graphอีกต่อไป เราจะให้การสนับสนุนด้านเทคนิคและการอัปเดตความปลอดภัยต่อไป แต่จะไม่มีการอัปเดตฟีเจอร์อีกต่อไป

**ตั้งแต่วันที่ 30 มิถุนายน 2022** เราจะสิ้นสุดการสนับสนุน ADAL และ Azure AD Graph และจะไม่มีการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยอีกต่อไป

แอปที่ใช้ ADAL บนเวอร์ชัน OS ที่มีอยู่จะยังคงสามารถใช้งานต่อหลังจากนี้ แต่ *จะไม่รับการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัย* ใดๆ

แอปที่ใช้ Azure AD Graphหลังจากนี้อาจไม่ได้รับการตอบกลับจากจุดสิ้นสุด Azure AD Graphอีกต่อไป

**การโยกย้าย ADAL**

เราขอแนะนนะ [ให้อัปเดตเป็น Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)ซึ่งมีฟีเจอร์ล่าสุดและการอัปเดตความปลอดภัย

ถ้าคุณใช้งานแอป Microsoft ทราบว่า Microsoft อยู่ในกระบวนการโยกย้ายแอปพลิเคชันไปยัง MSAL ภายในวันกําหนดสิ้นสุดการสนับสนุน เพื่อให้แน่ใจว่าพวกเขาจะได้รับประโยชน์จากการปรับปรุงความปลอดภัยและฟีเจอร์ของ MSAL ที่ต่อเนื่อง

สำหรับข้อมูลเพิ่มเติม ให้ดู:

1. [อ่าน ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [เรียนรู้เกี่ยวกับวิธีการโยกย้ายแอปตามแพลตฟอร์ม](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. ถ้าคุณต้องการความช่วยเหลือในการเข้าใจว่าแอปใดของคุณใช้ ADAL เราขอแนะนนะให้คุณตรวจสอบโค้ดต้นฉบับของแอปทั้งหมด และถ้าสามารถเข้าใจได้ ให้ติดต่อผู้ให้บริการ ISVs หรือแอป ฝ่ายสนับสนุนของ Microsoft ยังสามารถแสดงรายการแอปที่ไม่ใช่ Microsoft ADAL ทั้งหมดในผู้เช่าของคุณ

**การโยกย้าย AAD Graph**

สําหรับแอปพลิเคชันที่ใช้ Azure AD Graph ให้ปฏิบัติตามแนวทางของเราเพื่อโยกย้าย[แอป Azure AD Graph ไปยัง Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [รายการตรวจสอบการโยกย้ายของเราให้จุดเริ่มต้น](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. พอร์ทัลการลงทะเบียนแอป Azure ของคุณจะแสดงแอปพลิเคชันที่ใช้ AAD Graph เราขอแนะนนะให้คุณตรวจสอบโค้ดต้นฉบับของแอปของคุณทั้งหมด และถ้ามี ให้ติดต่อผู้ให้บริการ ISVs หรือแอปรายใดก็ได้ ฝ่ายสนับสนุนของ Microsoft ยังสามารถให้รายการของ AAD ทั้งหมดGraphการใช้งานในผู้เช่าของคุณ
3. เพื่อให้แอปของคุณเข้าถึงข้อมูลใน Microsoft Graphหรือผู้ดูแลระบบต้องให้สิทธิ์ที่ถูกต้องผ่านทางกระบวนการการยินยอม การอ้างอิง[สิทธิ์Graphของ Microsoft](https://docs.microsoft.com/graph/permissions-reference)จะแสดงรายการสิทธิ์ที่เกี่ยวข้องกับชุดหลักของ Microsoft Graph API แต่ละรายการ นอกจากนี้ยังมีแนวทางเกี่ยวกับวิธีการใช้สิทธิ์
