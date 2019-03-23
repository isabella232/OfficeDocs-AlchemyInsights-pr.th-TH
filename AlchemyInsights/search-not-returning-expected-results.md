---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776100"
---
# <a name="content-search-not-returning-expected-results"></a>ค้นหาเนื้อหาที่ไม่ส่งกลับผลลัพธ์ที่คาดไว้

เมื่อรันการค้นหาเนื้อหาจาก & Office 365 Security Center การปฏิบัติตามกฎระเบียบ คุณอาจได้รับผลลัพธ์การค้นหาที่ไม่คาดคิด พิจารณาสิ่งต่อไปนี้ที่สามารถส่งผลกระทบต่อผลลัพธ์การค้นหาของคุณ:

- **ตำแหน่งที่ตั้งเนื้อหาและเงื่อนไขการค้นหา**: ตรวจสอบว่า คุณได้เลือกตำแหน่งที่ตั้งเนื้อหาที่เหมาะสม และเงื่อนไขการค้นหา ถ้าคุณเรียกใช้การค้นหาที่มีขนาดใหญ่ (มีหลายตำแหน่งที่ตั้ง), พิจารณาเป็นการแบ่งเป็นหลายการค้นหา

- **ดัชนีรายการบางส่วน**:[ดัชนีสินค้าบางส่วน](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)จากกล่องจดหมายที่รวมอยู่ในผลลัพธ์การค้นหาที่ประเมิน อย่างไรก็ตาม สินค้าบางส่วนมีการทำดัชนีจากไซต์ SharePoint และ OneDrive จะไม่ถูกรวมในการประเมินการค้นหา

- **ความล้มเหลวในการค้นหา**: เมื่อค้นหาจำนวนมากกล่องจดหมาย (กล่องจดหมายมากกว่า 100000), คุณอาจได้รับข้อผิดพลาดค้นหา ด้วยรหัสข้อผิดพลาดเช่น CS008 009 และ CS012-002 โดย) ได้ ในกรณีนี้ ลองการค้นหาตำแหน่งที่ตั้งเนื้อหาที่ล้มเหลวเท่านั้นอีกครั้ง ดู[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)สำหรับข้อมูลเพิ่มเติม
