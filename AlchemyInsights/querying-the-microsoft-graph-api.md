---
title: การสอบถาม API ของ Microsoft Graph
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974688"
---
# <a name="querying-the-microsoft-graph-api"></a>การสอบถาม API ของ Microsoft Graph

หัวข้อนี้ยังอาจนำไปใช้กับนักพัฒนายังคงใช้ Azure AD Graph API อย่างไรก็ตาม **ขอแนะนำให้คุณ** ใช้ Microsoft Graph สำหรับสถานการณ์สมมติของไดเรกทอรีข้อมูลประจำตัวและการจัดการการเข้าถึงทั้งหมดของคุณ

**ปัญหาเกี่ยวกับการรับรองความถูกต้องหรือการอนุญาต**

- ถ้าแอปของคุณไม่ **สามารถรับโทเค็น** การโทรถึง microsoft graph ได้ให้เลือก **ปัญหาเกี่ยวกับการรับโทเค็นการเข้าถึง (การรับรองความถูกต้อง)** ประเภท Microsoft Graph เพื่อรับความช่วยเหลือและการสนับสนุนที่เฉพาะเจาะจงมากขึ้นในหัวข้อนี้
- ถ้าแอปของคุณได้ **รับข้อผิดพลาด** ในการอนุญาตให้ใช้งาน๔๐๑หรือ๔๐๓เมื่อโทรหา microsoft graph ให้เลือกประเภทการ **รับข้อผิดพลาดในการปฏิเสธการเข้าถึง (การอนุญาต)** Microsoft Graph API เพื่อรับความช่วยเหลือและการสนับสนุนที่เฉพาะเจาะจงมากขึ้นในหัวข้อนี้

**ฉันต้องการใช้ Microsoft Graph แต่ไม่แน่ใจว่าจะเริ่มต้นที่ใด**

เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับ Microsoft Graph ให้ดู:

- [ภาพรวมของ Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [ภาพรวมของการจัดการข้อมูลประจำตัวและการเข้าถึงใน Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [การเริ่มต้นใช้งานแอป Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** -ทดสอบ Microsoft graph APIs ในผู้เช่าของคุณหรือผู้เช่าสาธิต

**ฉันต้องการใช้ Microsoft Graph แต่สนับสนุนไดเรกทอรี v1.0 ที่ฉันจำเป็นต้องใช้**

Microsoft Graph เป็น API ที่แนะนำสำหรับไดเรกทอรีข้อมูลประจำตัวและการจัดการการเข้าถึง อย่างไรก็ตามยังมีช่องว่างไม่กี่ช่องระหว่างสิ่งที่เป็นไปได้ในกราฟโฆษณา Azure และ Microsoft Graph ตรวจทานบทความต่อไปนี้ซึ่งเน้นความแตกต่างล่าสุดสำหรับความช่วยเหลือในตัวเลือกของคุณ:

- [ความแตกต่างของชนิดทรัพยากรระหว่างกราฟ AD Azure และ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [ความแตกต่างของคุณสมบัติระหว่างกราฟโฆษณา Azure และ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [ความแตกต่างของวิธีการระหว่าง Azure AD และ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**เมื่อฉันสอบถามวัตถุ *ผู้ใช้* หลายคุณสมบัติจะหายไป**

`GET https://graph.microsoft.com/v1.0/users` ส่งกลับเฉพาะที่พัก11แห่งเนื่องจาก Microsoft Graph จะเลือกชุดของคุณสมบัติของ *ผู้ใช้* ที่จะส่งกลับเป็นค่าเริ่มต้น ถ้าคุณต้องการคุณสมบัติของ *ผู้ใช้* อื่นให้ใช้ $select เพื่อเลือกคุณสมบัติของแอปพลิเคชันที่คุณต้องการ ลองใช้งานใน **Microsoft Graph Explorer** ก่อน

**ค่าคุณสมบัติของผู้ใช้บางค่าเป็น *null* แม้ว่าฉันจะได้รับการตั้งค่า**

คำอธิบายที่เป็นไปได้มากที่สุดคือแอปพลิเคชันที่ได้รับอนุญาตให้ *ผู้ใช้ ReadBasic* การดำเนินการนี้จะช่วยให้แอปพลิเคชันอ่านคุณสมบัติของผู้ใช้ที่จำกัดและส่งกลับค่าคุณสมบัติอื่นๆทั้งหมดเป็น null แม้ว่าจะได้รับการตั้งค่าก่อนหน้านี้แล้ว ลองให้สิทธิ์ผู้ใช้แอปพลิเคชัน *อ่านสิทธิ์ทั้งหมด* แทน

สำหรับข้อมูลเพิ่มเติมให้ดูที่[สิทธิ์ของผู้ใช้ Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**ฉันมีปัญหาในการใช้พารามิเตอร์คิวรี OData เพื่อกรองข้อมูลในคำขอของฉัน**

ในขณะที่ Microsoft Graph สนับสนุนพารามิเตอร์แบบสอบถาม OData หลายพารามิเตอร์เหล่านั้นจะไม่ได้รับการสนับสนุนอย่างสมบูรณ์โดยบริการไดเรกทอรี (แหล่งข้อมูลที่สืบทอดมาจาก *directoryObject*) ใน Microsoft Graph ข้อจำกัดเดียวกันกับที่มีอยู่ในกราฟโฆษณา Azure ได้รับการยืนยันสำหรับส่วนใหญ่ใน Microsoft Graph:

1. **ไม่ได้รับการสนับสนุน**: $count, $search และ $filter บนค่า *null* หรือ *ไม่ใช่ค่า null*
2. **ไม่ได้รับการสนับสนุน**: $filter บนคุณสมบัติบางอย่าง (โปรดดูที่หัวข้อทรัพยากรที่มีคุณสมบัติใดที่เอา)
3. **ไม่ได้รับการสนับสนุน**: การแบ่งหน้าการกรองและการเรียงลำดับในเวลาเดียวกัน
4. **ไม่ได้รับการสนับสนุน**: การกรองบนความสัมพันธ์ ตัวอย่างเช่นค้นหาสมาชิกทั้งหมดของกลุ่มวิศวกรรมที่อยู่ในสหราชอาณาจักร
5. การ **สนับสนุนบางส่วน**: $orderby บน *ผู้ใช้*(displayName และ userPrincipalName เท่านั้น) และ *กลุ่ม*
6. การ **สนับสนุนบางส่วน**: $filter (สนับสนุนเฉพาะ *eq*, startswith *หรือ*, *and และ* จำกัด) การสนับสนุน $expand (การขยายความสัมพันธ์ของวัตถุเดี่ยวจะส่งกลับความสัมพันธ์ทั้งหมดแต่การขยายคอลเลกชันของความสัมพันธ์ของวัตถุจะถูกจำกัด) 

สำหรับข้อมูลเพิ่มเติมให้ดูที่การกำหนดค่าการ [ตอบสนองด้วยพารามิเตอร์คิว](https://docs.microsoft.com/graph/query-parameters)รี

**API ที่ฉันกำลังโทรไม่ทำงาน-ฉันสามารถทำการทดสอบเพิ่มเติมได้จากที่ใด**

**Microsoft Graph Explorer** -ทดสอบ Microsoft graph APIs ในผู้เช่าของคุณหรือผู้เช่าสาธิตและยังตรวจสอบ **แบบสอบถามตัวอย่าง** ใน Microsoft Graph explorer

**เมื่อฉันทำแบบสอบถามสำหรับข้อมูลดูเหมือนว่าฉันได้รับชุดข้อมูลที่ไม่สมบูรณ์กลับมา**

ถ้าคุณกำลังทำการสอบถามคอลเลกชัน (เช่น *ผู้ใช้*) Microsoft Graph จะใช้ขีดจำกัดของหน้าบนเซิร์ฟเวอร์เพื่อให้ผลลัพธ์จะถูกส่งกลับโดยใช้ขนาดหน้าเริ่มต้นเสมอ แอปของคุณควรคาดหวังให้หน้าผ่านคอลเลกชันที่ส่งกลับจากบริการนั้นเสมอ

สำหรับข้อมูลเพิ่มเติม ให้ดูที่

- [แนวทางปฏิบัติที่ดีที่สุดของ Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [การแบ่งหน้าข้อมูล Microsoft Graph ในแอปของคุณ](https://docs.microsoft.com/graph/paging)

**แอปของฉันช้าเกินไปและยังได้รับปริมาณ ฉันสามารถทำการปรับปรุงอะไรได้บ้าง**

ทั้งนี้ขึ้นอยู่กับสถานการณ์ของคุณมีหลายตัวเลือกที่แตกต่างกันในการขายทิ้งของคุณเพื่อทำให้แอปพลิเคชันของคุณมีประสิทธิภาพมากขึ้นและในบางกรณีอาจมีแนวโน้มที่จะปริมาณโดยบริการ (เมื่อคุณกำลังทำการโทรมากเกินไป)

เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่:

- [แนวทางปฏิบัติที่ดีที่สุดของ Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [การร้องขอ Batching](https://docs.microsoft.com/graph/json-batching)
- [ติดตามการเปลี่ยนแปลงผ่านคิวรีของเดลต้า](https://docs.microsoft.com/graph/delta-query-overview)
- [รับการแจ้งเตือนการเปลี่ยนแปลงผ่าน webhooks](https://docs.microsoft.com/graph/webhooks)
- [คำแนะนำการควบคุมปริมาณ](https://docs.microsoft.com/graph/throttling)

**ฉันจะค้นหาข้อมูลเพิ่มเติมเกี่ยวกับข้อผิดพลาดและปัญหาที่ทราบได้ที่ไหน**

- [ข้อมูลการตอบกลับข้อผิดพลาดของ Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [ปัญหาที่ทราบแล้วเกี่ยวกับ Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**ฉันจะตรวจสอบสถานะของบริการที่พร้อมใช้งานและการเชื่อมต่อได้ที่ใด**

ความพร้อมใช้งานของบริการและการเชื่อมต่อของบริการพื้นฐานที่สามารถเข้าถึงได้ผ่านทาง Microsoft Graph จะส่งผลกระทบต่อความพร้อมใช้งานและประสิทธิภาพการทำงานโดยรวมของ Microsoft Graph

- สำหรับสถานภาพบริการของ Azure Active Directory ให้ตรวจสอบสถานะของ **ความปลอดภัย + บริการข้อมูลประจำตัว** ที่แสดงรายการอยู่ใน [หน้าสถานะ Azure](https://azure.microsoft.com/status/)
- สำหรับบริการ Office ที่เกี่ยวข้องกับ Microsoft Graph ให้ตรวจสอบสถานะของบริการที่แสดงรายการอยู่ใน[แดชบอร์ดความสมบูรณ์ของบริการ Office](https://portal.office.com/adminportal/home#/servicehealth)
