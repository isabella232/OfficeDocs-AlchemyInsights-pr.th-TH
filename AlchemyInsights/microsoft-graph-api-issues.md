---
title: ปัญหาของ Microsoft Graph API
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975912"
---
# <a name="microsoft-graph-api-issues"></a>ปัญหาของ Microsoft Graph API

หัวข้อนี้ยังสามารถใช้กับนักพัฒนาที่ยังคงใช้ Azure AD Graph API ได้ อย่างไรก็ตาม ขอแ **นะGraph** ให้คุณใช้ Microsoft Graphสถานการณ์การจัดการไดเรกทอรี ข้อมูลเฉพาะตัว และการเข้าถึงทั้งหมด

**ปัญหาการรับรองความถูกต้องหรือการอนุญาต**

- ถ้าแอปของคุณ **ไม่สามารถ** รับโทเค็นเพื่อโทรหา Microsoft Graph ให้เลือก ปัญหาเกี่ยวกับการรับประเภทโทเค็นการเข้าถึง (การรับรองความถูกต้อง **)** Microsoft Graph เพื่อรับวิธีใช้และการสนับสนุนที่เฉพาะเจาะจงเพิ่มเติมเกี่ยวกับหัวข้อนี้
- ถ้าแอปของคุณได้รับ **ข้อผิดพลาดในการอนุญาต 401 หรือ 403** ครั้งเมื่อโทรหา Microsoft Graph ให้เลือกประเภท รับการเข้าถึงถูกปฏิเสธ **(การอนุญาต)** Microsoft Graph API เพื่อรับความช่วยเหลือและการสนับสนุนที่เฉพาะเจาะจงเพิ่มเติมเกี่ยวกับหัวข้อนี้

**ฉันต้องการใช้ Microsoft Graph แต่ไม่แน่ใจว่าจะเริ่มที่ไหน**

- [ภาพรวมของ Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [ภาพรวมของการจัดการข้อมูลเฉพาะตัวและการเข้าถึงใน Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [เริ่มต้นใช้งานการสร้างแอป Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - ทดสอบ API ของ Microsoft Graph ในผู้เช่าของคุณหรือผู้เช่าการสาธิต

**ฉันต้องการใช้ Microsoft Graph แต่สนับสนุน API ไดเรกทอรี v1.0 ที่ฉันต้องใช้หรือไม่**

Microsoft Graph คือ API ที่แนะนาให้ใช้ในการจัดการไดเรกทอรี ข้อมูลเฉพาะตัว และการจัดการการเข้าถึง อย่างไรก็ตาม ยังคงมีช่องว่างระหว่างสิ่งที่เป็นไปได้ใน Azure AD Graphและ Microsoft Graph ตรวจทานบทความต่อไปนี้ ซึ่งจะเน้นความแตกต่างล่าสุดเพื่อช่วยเหลือในตัวเลือกของคุณ:

- [ความแตกต่างของชนิดทรัพยากรระหว่าง Azure AD Graph และ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [ความแตกต่างของคุณสมบัติระหว่าง Azure AD Graph กับ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [ความแตกต่างระหว่าง Azure AD และ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API ที่ฉันโทรไม่มีประสิทธิภาพ ฉันจะทดสอบเพิ่มเติมได้ที่ไหน**

**Microsoft Graph Explorer** - ทดสอบ Microsoft Graph API ในผู้เช่าของคุณหรือผู้เช่าการสาธิต และตรวจสอบคิวรีตัวอย่างใน Microsoft Graph Explorer

**แอปของฉันช้าเกินไปและถูกควบคุมปริมาณ ฉันสามารถปรับปรุงอะไรได้บ้าง**

โดยขึ้นอยู่กับสถานการณ์ของคุณ มีตัวเลือกที่หลากหลายเพื่อให้แอปพลิเคชันมีประสิทธิภาพมากขึ้น และในบางกรณีมีแนวโน้มที่จะถูกควบคุมปริมาณโดยบริการน้อยลง (เมื่อคุณโทรมากเกินไป)

- [แนวทางปฏิบัติGraphของ Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [การร้องขอชุดการโยกย้าย](https://docs.microsoft.com/graph/json-batching)
- [ติดตามการเปลี่ยนแปลงผ่านคิวรีแบบใช้เลือกข้อมูล](https://docs.microsoft.com/graph/delta-query-overview)
- [รับการแจ้งเตือนเกี่ยวกับการเปลี่ยนแปลงผ่านเว็บ](https://docs.microsoft.com/graph/webhooks)
- [แนวทางการควบคุมปริมาณ](https://docs.microsoft.com/graph/throttling)

**ฉันจะค้นหาข้อมูลเพิ่มเติมเกี่ยวกับข้อผิดพลาดและปัญหาที่ทราบได้ที่ไหน**

- [ข้อมูลการGraphข้อผิดพลาดของ Microsoft](https://docs.microsoft.com/graph/errors)
- [ปัญหาที่ทราบแล้วของ Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**ฉันจะตรวจสอบสถานะความพร้อมใช้งานของบริการและการเชื่อมต่อได้ที่ไหน**

ความพร้อมใช้งานของบริการและการเชื่อมต่อบริการที่มีอยู่ที่สามารถเข้าถึงได้ผ่านทาง Microsoft Graph อาจส่งผลต่อความพร้อมใช้งานและประสิทธิภาพโดยรวมของ Microsoft Graph

- For Azure Active Directory service health, check the status of **Security + Identity services** listed in the Azure status [page](https://azure.microsoft.com/status/).
- For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).

ข้อผิดพลาดGraphการอนุญาตของ Microsoft อาจเกิดจากปัญหาต่างๆ มากมาย โดยส่วนใหญ่จะสร้างข้อผิดพลาด 401 หรือ 403 ตัวอย่างเช่น สิ่งต่อไปนี้อาจก่อให้เกิดข้อผิดพลาดในการตรวจสอบได้ทั้งหมด:

- โฟล [ว์การรับโทเค็นการเข้าถึงที่ไม่ถูกต้อง](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- กําหนดค่าขอบเขต [สิทธิ์ไม่ดี](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- ไม่มีความยินยอม[](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***การสิ้นสุดการสนับสนุนAzure Active Directory (ADAL) และ Azure AD Graph API (AAD Graph)***

**ตั้งแต่วันที่ 30 มิถุนายน 2020** เราจะไม่เพิ่มฟีเจอร์ใหม่ใดๆ ลงใน ADAL และ Azure AD Graphอีกต่อไป เราจะให้การสนับสนุนด้านเทคนิคและการอัปเดตความปลอดภัยต่อไป แต่จะไม่มีการอัปเดตฟีเจอร์อีกต่อไป

**ตั้งแต่วันที่ 30 มิถุนายน 2022** เราจะสิ้นสุดการสนับสนุน ADAL และ Azure AD Graph และจะไม่มีการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยอีกต่อไป

แอปที่ใช้ ADAL บนเวอร์ชัน OS ที่มีอยู่จะยังคงสามารถใช้งานต่อหลังจากนี้ แต่ *จะไม่รับการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัย* ใดๆ

แอปที่ใช้ Azure AD Graphหลังจากนี้อาจไม่ได้รับการตอบกลับจากจุดสิ้นสุด Azure AD Graphอีกต่อไป

**การโยกย้าย ADAL**

เราขอแนะนนะ [ให้อัปเดตเป็น Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)ซึ่งมีฟีเจอร์ล่าสุดและการอัปเดตความปลอดภัย

ถ้าคุณใช้งานแอป Microsoft ทราบว่า Microsoft อยู่ในกระบวนการโยกย้ายแอปพลิเคชันไปยัง MSAL ภายในวันกําหนดสิ้นสุดการสนับสนุน เพื่อให้แน่ใจว่าพวกเขาจะได้รับประโยชน์จากการปรับปรุงความปลอดภัยและฟีเจอร์ที่ MSAL มีอย่างต่อเนื่อง

1. [อ่าน ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [เรียนรู้เกี่ยวกับวิธีการโยกย้ายแอปตามแพลตฟอร์ม](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. ถ้าคุณต้องการความช่วยเหลือในการเข้าใจว่าแอปใดของคุณใช้ ADAL เราขอแนะนนะให้คุณตรวจสอบโค้ดต้นฉบับของแอปทั้งหมด และถ้าสามารถเข้าใจได้ ให้ติดต่อผู้ให้บริการ ISVs หรือแอป ฝ่ายสนับสนุนของ Microsoft ยังสามารถแสดงรายการแอปที่ไม่ใช่ Microsoft ADAL ทั้งหมดในผู้เช่าของคุณ

**การโยกย้าย AAD Graph**

สําหรับแอปพลิเคชันที่ใช้ Azure AD Graph ให้ปฏิบัติตามแนวทางของเราเพื่อโยกย้าย[แอป Azure AD Graph ไปยัง Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [รายการตรวจสอบการโยกย้ายของเราให้จุดเริ่มต้น](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. พอร์ทัลการลงทะเบียนแอป Azure ของคุณจะแสดงแอปพลิเคชันที่ใช้ AAD Graph เราขอแนะนนะให้คุณตรวจสอบโค้ดต้นฉบับของแอปของคุณทั้งหมด และถ้ามี ให้ติดต่อผู้ให้บริการ ISVs หรือแอปรายใดก็ได้ ฝ่ายสนับสนุนของ Microsoft ยังสามารถให้รายการของ AAD ทั้งหมดGraphการใช้งานในผู้เช่าของคุณ
3. เพื่อให้แอปของคุณเข้าถึงข้อมูลใน Microsoft Graphหรือผู้ดูแลระบบต้องให้สิทธิ์ที่ถูกต้องผ่านทางกระบวนการการยินยอม การอ้างอิง[สิทธิ์Graphของ Microsoft](https://docs.microsoft.com/graph/permissions-reference)จะแสดงรายการสิทธิ์ที่เกี่ยวข้องกับชุดหลักของ Microsoft Graph API แต่ละรายการ นอกจากนี้ยังมีแนวทางเกี่ยวกับวิธีการใช้สิทธิ์
