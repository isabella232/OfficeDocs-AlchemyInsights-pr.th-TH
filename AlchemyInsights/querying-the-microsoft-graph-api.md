---
title: การสอบถามเกี่ยวกับ Microsoft Graph API
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923258"
---
# <a name="querying-the-microsoft-graph-api"></a>การสอบถามเกี่ยวกับ Microsoft Graph API

หัวข้อนี้ยังสามารถใช้กับนักพัฒนาที่ยังคงใช้ Azure AD Graph API ได้ อย่างไรก็ตาม ขอแ **นะGraph** ให้คุณใช้ Microsoft Graphสถานการณ์การจัดการไดเรกทอรี ข้อมูลเฉพาะตัว และการเข้าถึงทั้งหมด

**ปัญหาการรับรองความถูกต้องหรือการอนุญาต**

- ถ้าแอปของคุณ **ไม่สามารถ** รับโทเค็นเพื่อโทรหา Microsoft Graph ให้เลือก ปัญหาเกี่ยวกับการรับประเภทโทเค็นการเข้าถึง (การรับรองความถูกต้อง **)** Microsoft Graph เพื่อรับวิธีใช้และการสนับสนุนที่เฉพาะเจาะจงเพิ่มเติมเกี่ยวกับหัวข้อนี้
- ถ้าแอปของคุณได้รับ **ข้อผิดพลาดในการอนุญาต 401 หรือ 403** ครั้งเมื่อโทรหา Microsoft Graph ให้เลือกประเภท รับการเข้าถึงถูกปฏิเสธ **(การอนุญาต)** Microsoft Graph API เพื่อรับความช่วยเหลือและการสนับสนุนที่เฉพาะเจาะจงเพิ่มเติมเกี่ยวกับหัวข้อนี้

**ฉันต้องการใช้ Microsoft Graph แต่ไม่แน่ใจว่าจะเริ่มที่ไหน**

เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับGraph Microsoft ให้ดู:

- [ภาพรวมของ Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [ภาพรวมของการจัดการข้อมูลเฉพาะตัวและการเข้าถึงใน Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [เริ่มต้นใช้งานการสร้างแอป Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - ทดสอบ API ของ Microsoft Graph ในผู้เช่าของคุณหรือผู้เช่าการสาธิต

**ฉันต้องการใช้ Microsoft Graph แต่สนับสนุน API ไดเรกทอรี v1.0 ที่ฉันต้องใช้หรือไม่**

Microsoft Graph คือ API ที่แนะนาให้ใช้ในการจัดการไดเรกทอรี ข้อมูลเฉพาะตัว และการจัดการการเข้าถึง อย่างไรก็ตาม ยังคงมีช่องว่างระหว่างสิ่งที่เป็นไปได้ใน Azure AD Graphและ Microsoft Graph ตรวจทานบทความต่อไปนี้ ซึ่งจะเน้นความแตกต่างล่าสุดเพื่อช่วยเหลือในตัวเลือกของคุณ:

- [ความแตกต่างของชนิดทรัพยากรระหว่าง Azure AD Graph และ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [ความแตกต่างของคุณสมบัติระหว่าง Azure AD Graph กับ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [ความแตกต่างระหว่าง Azure AD และ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**When I query the *user* object, many of its properties are missing**

`GET https://graph.microsoft.com/v1.0/users`จะส่งกลับคุณสมบัติเพียง 11 Graph Microsoft จะเลือกชุดคุณสมบัติ *ผู้ใช้* เริ่มต้นเพื่อส่งกลับโดยอัตโนมัติ If you need other *user* properties, use $select to pick the properties your application needs. ลองค้นหาใน **Microsoft Graph Explorer** ก่อน

**ค่าคุณสมบัติผู้ใช้บาง *ค่าเป็น* Null แม้ว่าฉันจะทราบว่าค่าเหล่านั้นถูกตั้งค่าแล้ว**

คําอธิบายที่เป็นไปได้มากที่สุดคือแอปพลิเคชันได้รับสิทธิ์ *User.ReadBasic.All* ซึ่งช่วยให้แอปพลิเคชันสามารถอ่านชุดคุณสมบัติผู้ใช้ที่จํากัด คืนค่าคุณสมบัติอื่นๆ ทั้งหมดเป็น Null แม้ว่าคุณสมบัติเหล่านั้นจะถูกตั้งค่าไว้ก่อนหน้า ลองให้สิทธิ์ *User.Read.All* ของแอปพลิเคชันแทน

For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**ฉันมีปัญหาในการใช้พารามิเตอร์คิวรี OData เพื่อกรองข้อมูลในการร้องขอของฉัน**

ในขณะที่ Microsoft Graph สนับสนุนพารามิเตอร์คิวรี OData ที่หลากหลาย พารามิเตอร์เหล่านั้นมากมายไม่ได้รับการสนับสนุนอย่างสมบูรณ์โดยบริการไดเรกทอรี (ทรัพยากรที่สืบทอดจาก *directoryObject*) ใน Microsoft Graph ข้อจํากัดเดียวกันกับที่มีอยู่ในบัญชี Azure AD Graphยังคงมีอยู่ส่วนใหญ่ใน Microsoft Graph:

1. **ไม่สนับสนุน : $count,**$search $filter *null* หรือไม่ *มีค่า* Null
2. **ไม่สนับสนุน:**$filterคุณสมบัติบางอย่าง (ดูหัวข้อทรัพยากรเกี่ยวกับคุณสมบัติที่สามารถกรองได้)
3. **ไม่สนับสนุน :** การแบ่งหน้า การกรอง และการเรียงล.ก. พร้อมกัน
4. **ไม่สนับสนุน**: การกรองความสัมพันธ์ ตัวอย่างเช่น - ค้นหาสมาชิกทั้งหมดของกลุ่มวิศวกรรมที่อยู่ในสหราชอาณาจักร
5. **การสนับสนุนบางส่วน**: *$orderbyผู้ใช้* (displayName และ userPrincipalName เท่านั้น) และ *กลุ่ม*
6. **การสนับสนุนบางส่วน**: $filter (สนับสนุนเฉพาะ *eq**เท่านั้น* เริ่มต้นด้วย *หรือ* และ และจํากัด ) สนับสนุน $expand (การขยายความสัมพันธ์ของวัตถุเดียวจะส่งกลับความสัมพันธ์ทั้งหมด แต่การขยายคอลเลกชันของความสัมพันธ์ของวัตถุมีจํากัด)

For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).

**API ที่ฉันโทรไม่ได้ผล ฉันจะทดสอบเพิ่มเติมได้ที่ไหน**

**Microsoft Graph Explorer** - ทดสอบ Microsoft Graph API ในผู้เช่าของคุณหรือผู้เช่าการสาธิต และตรวจสอบคิวรีตัวอย่างใน Microsoft Graph Explorer

**เมื่อฉันคิวรีข้อมูล ดูเหมือนว่าฉันได้รับชุดข้อมูลที่ไม่สมบูรณ์**

ถ้าคุณคิวรีคอลเลกชัน (เช่น *ผู้ใช้*) Microsoft Graph จะใช้ขีดจํากัดหน้าที่ฝั่งเซิร์ฟเวอร์ ดังนั้นผลลัพธ์จะถูกส่งกลับด้วยขนาดหน้าเริ่มต้นเสมอ แอปของคุณควรคาดว่าจะเปิดดูคอลเลกชันที่ส่งกลับจากบริการเสมอ

สำหรับข้อมูลเพิ่มเติม ให้ดู:

- [แนวทางปฏิบัติGraphของ Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [การแบ่งหน้า Microsoft Graphข้อมูลในแอปของคุณ](https://docs.microsoft.com/graph/paging)

**แอปของฉันช้าเกินไปและถูกควบคุมปริมาณ ฉันสามารถปรับปรุงอะไรได้บ้าง**

โดยขึ้นอยู่กับสถานการณ์ของคุณ มีตัวเลือกต่างๆ มากมายเพื่อที่แอปพลิเคชันจะมีประสิทธิภาพมากขึ้น และในบางกรณีก็มีแนวโน้มที่จะถูกควบคุมปริมาณโดยบริการน้อยลง (เมื่อคุณโทรมากเกินไป)

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู:

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
