---
title: 1491-ค้นหาไม่ส่งคืนผลลัพธ์ที่คาดไว้
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709246"
---
# <a name="content-search-not-returning-expected-results"></a>การค้นหาเนื้อหาไม่ส่งกลับผลลัพธ์ที่คาดไว้

เมื่อเรียกใช้การค้นหาเนื้อหาจาก Microsoft 365 &ศูนย์การปฏิบัติตามกฎระเบียบ พิจารณาสิ่งต่อไปนี้ที่อาจส่งผลต่อผลการค้นหาของคุณ

- **ตําแหน่งที่ตั้งเนื้อหาและเงื่อนไขการค้นหา**: ตรวจสอบให้แน่ใจว่าคุณได้เลือกตําแหน่งเนื้อหาที่เหมาะสมและเงื่อนไขการค้นหา หากคุณค้นหาข้อมูลจํานวนมาก (ที่มีหลายตําแหน่ง) ให้พิจารณาแยกการค้นหาออกเป็นหลายการค้นหา

- **รายการที่มีการทําดัชนีบางส่วน**:[รายการทําดัชนีบางส่วน](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)จากกล่องจดหมายจะรวมอยู่ในผลลัพธ์การค้นหาโดยประมาณ อย่างไรก็ตาม รายการทําดัชนีบางส่วนจากไซต์ใน SharePoint และ OneDrive จะไม่รวมอยู่ในการประเมินการค้นหา

- **ความล้มเหลวในการค้นหา**: เมื่อค้นหากล่องจดหมายจํานวนมาก (กล่องจดหมายมากกว่า 100,000 กล่อง) คุณอาจได้รับข้อผิดพลาดในการค้นหาที่มีรหัสข้อผิดพลาดเช่น CS008-009 และ CS012-002) ในกรณีนี้ ให้ลองค้นหาสําหรับตําแหน่งที่ตั้งเนื้อหาที่ล้มเหลวเท่านั้น ดู[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)สําหรับข้อมูลเพิ่มเติม
