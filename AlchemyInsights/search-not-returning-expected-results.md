---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052729"
---
# <a name="content-search-not-returning-expected-results"></a>การค้นหาเนื้อหาไม่ส่งกลับผลลัพธ์ที่คาดไว้

เมื่อเรียกใช้การค้นหาเนื้อหาจากศูนย์Microsoft 365การปฏิบัติตาม&ปฏิบัติตามข้อบังคับ คุณอาจได้รับผลลัพธ์การค้นหาที่ไม่คาดคิด พิจารณาสิ่งต่อไปนี้ที่อาจส่งผลต่อผลลัพธ์การค้นหาของคุณ:

- **สถานที่ของเนื้อหาและเงื่อนไขการค้นหา**: ตรวจสอบให้แน่ใจว่าคุณได้เลือกที่ตั้งเนื้อหาและเงื่อนไขการค้นหาที่เหมาะสม ถ้าคุณเรียกใช้การค้นหาขนาดใหญ่ (ที่มีหลายสถานที่) ให้พิจารณาแยกการค้นหาออกเป็นการค้นหาหลายรายการ

- **รายการที่ได้สร้างดัชนี** บางส่วน:  [รายการที่ได้](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) สร้างดัชนีบางส่วนจากกล่องจดหมายจะรวมอยู่ในผลลัพธ์การค้นหาโดยประมาณ อย่างไรก็ตาม รายการที่ถูกดัชนีบางส่วนจากไซต์ใน SharePoint OneDriveรายการนั้นจะไม่รวมอยู่ในการประเมินการค้นหา

- **การค้นหาล้มเหลว**: เมื่อค้นหากล่องจดหมายจํานวนมาก (กล่องจดหมายมากกว่า 100,000 กล่อง) คุณอาจได้รับข้อผิดพลาดการค้นหา ด้วยรหัสข้อผิดพลาด เช่น CS008-009 และ CS012-002) ในกรณีนี้ ให้ลองค้นหาเฉพาะกับที่ตั้งเนื้อหาที่ล้มเหลวเท่านั้น [ดู](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)บทความนี้เพื่อดูข้อมูลเพิ่มเติม
