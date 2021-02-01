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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063701"
---
# <a name="issues-with-authentication-libraries"></a>ปัญหาเกี่ยวกับไลบรารีการรับรองความถูกต้อง

1. [ไลบรารีการรับรองความถูกต้องแพลตฟอร์มข้อมูลเฉพาะตัวของ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) Microsoft แสดงรายการไลบรารีไคลเอ็นต์และ Middleware ที่ได้รับการสนับสนุนและเข้ากันได้ของ Microsoft
2. ไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL) สนับสนุนขั้นตอน [การรับรองความถูกต้องหลายอย่าง](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) เพื่อใช้ในสถานการณ์ของแอปพลิเคชันต่างๆ
3. เมื่อต้องการรับรองความถูกต้องและรับโทเค็น ให้คุณเตรียมใช้งานแอปพลิเคชันไคลเอ็นต์สาธารณะหรือแอปพลิเคชันที่เป็นความลับใหม่ในโค้ดของคุณ คุณสามารถตั้งค่าตัวเลือกการกําหนดค่าได้หลายตัวเลือกเมื่อคุณเตรียมใช้งานแอปไคลเอ็นต์ในไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL) เมื่อต้องการเรียนรู้เพิ่มเติม ดูตัวเลือก [การกําหนดค่า](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)แอปพลิเคชัน

**การสิ้นสุดการสนับสนุนของ Azure Active Directory Authentication Library (ADAL) และ Azure AD Graph API (AAD Graph)**

**ตั้งแต่วันที่ 30 มิถุนายน 2020** เราจะไม่เพิ่มฟีเจอร์ใหม่ใดๆ ลงใน ADAL และ Azure AD Graph อีกต่อไป เราจะให้การสนับสนุนด้านเทคนิคและการอัปเดตความปลอดภัยต่อ แต่จะไม่มีการอัปเดตฟีเจอร์อีกต่อไป

**ตั้งแต่วันที่ 30 มิถุนายน 2022** เราจะสิ้นสุดการสนับสนุน ADAL และ Azure AD Graph และจะไม่มีการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยอีกต่อไป

แอปที่ใช้ ADAL บนเวอร์ชัน OS ที่มีอยู่จะยังคงสามารถใช้งานต่อไปได้หลังจากนี้ *แต่จะไม่ได้รับการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัย* ใดๆ

แอปที่ใช้ Azure AD Graph หลังจากช่วงเวลานี้อาจไม่ได้รับการตอบกลับจากจุดสิ้นสุด Azure AD Graph อีกต่อไป

**การโยกย้าย ADAL**

เราขอแนะนนะ [ให้อัปเดตไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)ซึ่งมีฟีเจอร์ล่าสุดและการอัปเดตความปลอดภัย

ถ้าคุณใช้งานแอปของ Microsoft ทราบว่า Microsoft อยู่ในระหว่างกระบวนการโยกย้ายแอปพลิเคชันไปยัง MSAL ภายในวันที่สิ้นสุดการสนับสนุน เพื่อให้มั่นใจว่าแอปเหล่านั้นจะได้รับประโยชน์จากการรักษาความปลอดภัยและการปรับปรุงฟีเจอร์ที่ MSAL อย่างต่อเนื่อง

สำหรับข้อมูลเพิ่มเติม ให้ดูที่

1. [อ่าน ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [เรียนรู้เกี่ยวกับวิธีการโยกย้ายแอปตามแพลตฟอร์ม](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. ถ้าคุณต้องการความช่วยเหลือในการเข้าใจว่าแอปใดของคุณใช้ ADAL เราขอแนะนาให้คุณตรวจสอบโค้ดต้นฉบับของแอปของคุณทั้งหมด และถ้าสามารถใช้งานได้ ให้ติดต่อผู้ให้บริการ ISVs หรือแอปรายใดก็ได้ ฝ่ายสนับสนุนของ Microsoft ยังสามารถแสดงรายการของแอปที่ไม่ใช่ Microsoft ADAL ทั้งหมดในผู้เช่าของคุณ

**การโยกย้ายกราฟ AAD**

สําหรับแอปพลิเคชันที่ใช้ Azure AD Graph ให้ปฏิบัติตามแนวทางของเราเพื่อ[โยกย้ายแอป Azure AD Graph ไปยัง Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [รายการตรวจสอบการโยกย้ายของเราให้จุดเริ่มต้น](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. พอร์ทัลการลงทะเบียนแอป Azure ของคุณจะแสดงแอปพลิเคชันที่ใช้ AAD Graph เราขอแนะนนะให้คุณตรวจสอบรหัสต้นฉบับของแอปของคุณทั้งหมด และหากสามารถติดต่อผู้ให้บริการ ISVs หรือแอปใดก็ได้ ฝ่ายสนับสนุนของ Microsoft ยังสามารถแสดงรายการการใช้งาน AAD Graph ทั้งหมดในผู้เช่าของคุณ
3. เพื่อให้แอปของคุณเข้าถึงข้อมูลใน Microsoft Graph ผู้ใช้หรือผู้ดูแลระบบต้องให้สิทธิ์ที่ถูกต้องผ่านทางกระบวนการการยินยอม การอ้างอิง [สิทธิ์ของ Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) จะแสดงรายการสิทธิ์ที่เกี่ยวข้องกับแต่ละชุดหลักของ Microsoft Graph API นอกจากนี้ยังมีแนวทางเกี่ยวกับวิธีการใช้สิทธิ์
