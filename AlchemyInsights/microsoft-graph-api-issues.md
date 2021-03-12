---
title: ปัญหา Microsoft Graph API
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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714516"
---
# <a name="microsoft-graph-api-issues"></a>ปัญหา Microsoft Graph API

หัวข้อนี้ยังอาจใช้กับนักพัฒนาที่ยังคงใช้ Azure AD Graph API อย่างไรก็ตาม ขอแ **นะให้** คุณใช้ Microsoft Graph กับไดเรกทอรี ข้อมูลเฉพาะตัว และสถานการณ์การจัดการการเข้าถึงทั้งหมด

**ปัญหาการรับรองความถูกต้องหรือการอนุญาต**

- ถ้าแอปของคุณ **ไม่สามารถขอรับ** โทเค็นเพื่อโทรหา Microsoft Graph ได้ ให้เลือกปัญหาด้วยการรับประเภทโทเค็นการเข้าถึง (การรับรองความถูกต้อง **)** Microsoft Graph เพื่อรับความช่วยเหลือและการสนับสนุนที่เฉพาะเจาะจงมากขึ้นในหัวข้อนี้
- ถ้าแอปของคุณได้รับ **ข้อผิดพลาดการอนุญาต 401 หรือ 403** เมื่อโทรหา Microsoft Graph ให้เลือกประเภทการรับการเข้าถึงที่ถูกปฏิเสธข้อผิดพลาด **(การตรวจสอบ)** API ของ Microsoft Graph เพื่อรับความช่วยเหลือและการสนับสนุนที่เฉพาะเจาะจงมากขึ้นในหัวข้อนี้

**ฉันต้องการใช้ Microsoft Graph แต่ไม่แน่ใจว่าจะเริ่มต้นที่ไหน**

- [ภาพรวมของ Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [ภาพรวมของข้อมูลเฉพาะตัวและการจัดการการเข้าถึงใน Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [เริ่มต้นสร้างแอป Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - ทดสอบ API ของ Microsoft Graph ในผู้เช่าของคุณหรือผู้เช่าการสาธิต

**ฉันต้องการใช้ Microsoft Graph แต่สนับสนุน API ไดเรกทอรี v1.0 ที่ฉันต้องการหรือไม่**

Microsoft Graph คือ API ที่แนะนนะให้ในการจัดการไดเรกทอรี ข้อมูลเฉพาะตัว และการจัดการการเข้าถึง อย่างไรก็ตาม ยังคงมีช่องว่างบางอย่างระหว่างสิ่งที่เป็นไปได้ใน Azure AD Graph และ Microsoft Graph ตรวจทานบทความต่อไปนี้ ซึ่งเน้นความแตกต่างล่าสุดเพื่อช่วยเหลือในตัวเลือกของคุณ:

- [ความแตกต่างของชนิดทรัพยากรระหว่าง Azure AD Graph และ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [ความแตกต่างของคุณสมบัติระหว่าง Azure AD Graph และ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [ความแตกต่างของวิธีการระหว่าง Azure AD และ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API ที่ฉันโทรไม่ใช้งาน - ฉันจะทดสอบเพิ่มเติมได้ที่ไหน**

**Microsoft Graph Explorer** - ทดสอบ Microsoft Graph API ในผู้เช่าของคุณหรือผู้เช่าการสาธิต และตรวจสอบคิวรี **ตัวอย่าง** ใน Microsoft Graph Explorer

**แอปของฉันช้าเกินไปและถูกควบคุมปริมาณ ฉันสามารถปรับปรุงอะไรได้บ้าง**

ขึ้นอยู่กับสถานการณ์ของคุณ มีตัวเลือกที่หลากหลายเพื่อให้แอปพลิเคชันของคุณมีประสิทธิภาพมากขึ้น และในบางกรณี มีแนวโน้มที่จะถูกควบคุมปริมาณโดยบริการน้อยลง (เมื่อคุณโทรมากเกินไป)

- [หลักปฏิบัติที่ดีที่สุดของ Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [การร้องขอเป็นชุด](https://docs.microsoft.com/graph/json-batching)
- [ติดตามการเปลี่ยนแปลงผ่านคิวรีส่วนที่แตกต่าง](https://docs.microsoft.com/graph/delta-query-overview)
- [รับการแจ้งเตือนเกี่ยวกับการเปลี่ยนแปลงผ่าน Webhooks](https://docs.microsoft.com/graph/webhooks)
- [แนวทางการควบคุมปริมาณ](https://docs.microsoft.com/graph/throttling)

**ฉันจะหาข้อมูลเพิ่มเติมเกี่ยวกับข้อผิดพลาดและปัญหาที่ทราบได้ที่ไหน**

- [ข้อมูลการตอบสนองต่อข้อผิดพลาดของ Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [ปัญหาที่ทราบเกี่ยวกับ Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**ฉันจะตรวจสอบสถานะความพร้อมของบริการและการเชื่อมต่อได้ที่ไหน**

ความพร้อมใช้งานบริการและการเชื่อมต่อของบริการที่อยู่ภายใต้การเข้าถึงผ่านทาง Microsoft Graph สามารถส่งผลกระทบต่อความพร้อมใช้งานและประสิทธิภาพโดยรวมของ Microsoft Graph ได้

- สถานภาพบริการ Azure Active Directory ให้ตรวจสอบสถานะ **ของบริการความปลอดภัย +** ข้อมูลเฉพาะตัวที่แสดงใน [หน้าสถานะ Azure](https://azure.microsoft.com/status/)
- บริการ Office ที่มีส่วนร่วมใน Microsoft Graph ให้ตรวจสอบสถานะของบริการที่แสดงในแดชบอร์ด[สถานภาพบริการของ Office](https://portal.office.com/adminportal/home#/servicehealth)

ข้อผิดพลาดในการตรวจสอบ Microsoft Graph อาจเป็นผลจากปัญหาต่างๆ มากมาย ซึ่งส่วนใหญ่จะสร้างข้อผิดพลาด 401 หรือ 403 ตัวอย่างเช่น สิ่งต่อไปนี้อาจก่อให้เกิดข้อผิดพลาดในการตรวจสอบได้

- โฟล [ว์การรับโทเค็นการเข้าถึงที่ไม่ถูกต้อง](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- กําหนดขอบเขตสิทธิ์ [ได้ไม่ดี](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- ขาดความยินยอม[](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_สิ้นสุดการสนับสนุนของ Azure Active Directory Authentication Library (ADAL) และ Azure AD Graph API (AAD Graph)_* _

_*เริ่มต้นวันที่ 30 มิถุนายน 2020** เราจะไม่เพิ่มฟีเจอร์ใหม่ใดๆ ลงใน ADAL และ Azure AD Graph อีกต่อไป เราจะให้การสนับสนุนด้านเทคนิคและการอัปเดตความปลอดภัยต่อ แต่จะไม่มีการอัปเดตฟีเจอร์อีกต่อไป

**ตั้งแต่วันที่ 30 มิถุนายน 2022** เราจะสิ้นสุดการสนับสนุน ADAL และ Azure AD Graph และจะไม่มีการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยอีกต่อไป

แอปที่ใช้ ADAL บนเวอร์ชัน OS ที่มีอยู่จะยังคงสามารถใช้งานต่อไปได้หลังจากนี้ *แต่จะไม่ได้รับการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัย* ใดๆ

แอปที่ใช้ Azure AD Graph หลังจากช่วงเวลานี้อาจไม่ได้รับการตอบกลับจากจุดสิ้นสุด Azure AD Graph อีกต่อไป

**การโยกย้าย ADAL**

เราขอแนะนนะ [ให้อัปเดตไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)ซึ่งมีฟีเจอร์ล่าสุดและการอัปเดตความปลอดภัย

ถ้าคุณใช้งานแอปของ Microsoft ทราบว่า Microsoft อยู่ในระหว่างกระบวนการโยกย้ายแอปพลิเคชันไปยัง MSAL ภายในวันที่สิ้นสุดการสนับสนุน เพื่อให้มั่นใจว่าแอปเหล่านั้นจะได้รับประโยชน์จากการปรับปรุงความปลอดภัยและฟีเจอร์ที่ MSAL มีอย่างต่อเนื่อง

1. [อ่าน ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [เรียนรู้เกี่ยวกับวิธีการโยกย้ายแอปตามแพลตฟอร์ม](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. ถ้าคุณต้องการความช่วยเหลือในการเข้าใจว่าแอปใดของคุณใช้ ADAL เราขอแนะนาให้คุณตรวจสอบโค้ดต้นฉบับของแอปทั้งหมด และถ้าสามารถใช้งานได้ ให้ติดต่อผู้ให้บริการ ISVs หรือแอปรายใดก็ได้ ฝ่ายสนับสนุนของ Microsoft ยังสามารถแสดงรายการของแอปที่ไม่ใช่ Microsoft ADAL ทั้งหมดในผู้เช่าของคุณ

**การโยกย้ายกราฟ AAD**

สําหรับแอปพลิเคชันที่ใช้ Azure AD Graph ให้ปฏิบัติตามแนวทางของเราเพื่อ[โยกย้ายแอป Azure AD Graph ไปยัง Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [รายการตรวจสอบการโยกย้ายของเราให้จุดเริ่มต้น](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. พอร์ทัลการลงทะเบียนแอป Azure ของคุณจะแสดงแอปพลิเคชันที่ใช้ AAD Graph เราขอแนะนนะให้คุณตรวจสอบรหัสต้นฉบับของแอปของคุณทั้งหมด และหากสามารถติดต่อผู้ให้บริการ ISVs หรือแอปใดก็ได้ ฝ่ายสนับสนุนของ Microsoft ยังสามารถแสดงรายการการใช้งาน AAD Graph ทั้งหมดในผู้เช่าของคุณ
3. เพื่อให้แอปของคุณเข้าถึงข้อมูลใน Microsoft Graph ผู้ใช้หรือผู้ดูแลระบบต้องให้สิทธิ์ที่ถูกต้องผ่านทางกระบวนการการยินยอม การอ้างอิง [สิทธิ์ของ Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) จะแสดงรายการสิทธิ์ที่เกี่ยวข้องกับแต่ละชุดหลักของ Microsoft Graph API นอกจากนี้ยังมีแนวทางเกี่ยวกับวิธีการใช้สิทธิ์
