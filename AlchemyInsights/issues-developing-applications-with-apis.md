---
title: ปัญหาในการพัฒนาแอปพลิเคชันด้วย API
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
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013479"
---
# <a name="issues-developing-applications-with-apis"></a>ปัญหาในการพัฒนาแอปพลิเคชันด้วย API

เมื่อต้องการเริ่มต้นใช้งาน API Azure Active Directory Graph ให้ดู คู่มือเริ่มต้นใช้งานด่วน[ของ API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) Graph Azure AD หรือดูคู่มืออ้างอิง[Azure AD Graph API](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)แบบโต้ตอบ

**การสิ้นสุดการสนับสนุนAzure Active Directory (ADAL) และ Azure AD Graph API (AAD Graph)**

**ตั้งแต่วันที่ 30 มิถุนายน 2020** เราจะไม่เพิ่มฟีเจอร์ใหม่ใดๆ ลงใน ADAL และ Azure AD Graphอีกต่อไป เราจะให้การสนับสนุนด้านเทคนิคและการอัปเดตความปลอดภัยต่อไป แต่จะไม่มีการอัปเดตฟีเจอร์อีกต่อไป

**ตั้งแต่วันที่ 30 มิถุนายน 2022** เราจะสิ้นสุดการสนับสนุน ADAL และ Azure AD Graph และจะไม่มีการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยอีกต่อไป

แอปที่ใช้ ADAL บนเวอร์ชัน OS ที่มีอยู่จะยังคงสามารถใช้งานต่อหลังจากนี้ แต่จะไม่รับการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยใดๆ

แอปที่ใช้ Azure AD Graphหลังจากนี้อาจไม่ได้รับการตอบกลับจากจุดสิ้นสุด Azure AD Graphอีกต่อไป

**การโยกย้าย ADAL**

เราขอแนะนนะ [ให้อัปเดตเป็น Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)ซึ่งมีฟีเจอร์ล่าสุดและการอัปเดตความปลอดภัย

ถ้าคุณใช้งานแอป Microsoft ทราบว่า Microsoft อยู่ในกระบวนการโยกย้ายแอปพลิเคชันไปยัง MSAL ภายในวันกําหนดสิ้นสุดการสนับสนุน เพื่อให้แน่ใจว่าพวกเขาจะได้รับประโยชน์จากการปรับปรุงความปลอดภัยและฟีเจอร์ที่ต่อเนื่องของ MSAL

1. [อ่าน ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [เรียนรู้เกี่ยวกับวิธีการโยกย้ายแอปตามแพลตฟอร์ม](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. ถ้าคุณต้องการความช่วยเหลือในการเข้าใจว่าแอปใดของคุณใช้ ADAL เราขอแนะนนะให้คุณตรวจสอบโค้ดต้นฉบับของแอปทั้งหมด และถ้าสามารถเข้าใจได้ ให้ติดต่อผู้ให้บริการ ISVs หรือแอป ฝ่ายสนับสนุนของ Microsoft ยังสามารถแสดงรายการแอปที่ไม่ใช่ Microsoft ADAL ทั้งหมดในผู้เช่าของคุณ

**การโยกย้าย AAD Graph**

สําหรับแอปพลิเคชันที่ใช้ Azure AD Graph ให้ปฏิบัติตามแนวทางของเราเพื่อโยกย้าย[แอป Azure AD Graph ไปยัง Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [รายการตรวจสอบการโยกย้ายของเราให้จุดเริ่มต้น](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
1. พอร์ทัลการลงทะเบียนแอป Azure ของคุณจะแสดงแอปพลิเคชันที่ใช้ AAD Graph เราขอแนะนนะให้คุณตรวจสอบโค้ดต้นฉบับของแอปของคุณทั้งหมด และถ้ามี ให้ติดต่อผู้ให้บริการ ISVs หรือแอปรายใดก็ได้ ฝ่ายสนับสนุนของ Microsoft ยังสามารถให้รายการของ AAD ทั้งหมดGraphการใช้งานในผู้เช่าของคุณ
1. เพื่อให้แอปของคุณเข้าถึงข้อมูลใน Microsoft Graphหรือผู้ดูแลระบบต้องให้สิทธิ์ที่ถูกต้องผ่านทางกระบวนการการยินยอม การอ้างอิง[สิทธิ์Graphของ Microsoft](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true)จะแสดงรายการสิทธิ์ที่เกี่ยวข้องกับชุดหลักของ Microsoft Graph API แต่ละรายการ นอกจากนี้ยังมีแนวทางเกี่ยวกับวิธีการใช้สิทธิ์
