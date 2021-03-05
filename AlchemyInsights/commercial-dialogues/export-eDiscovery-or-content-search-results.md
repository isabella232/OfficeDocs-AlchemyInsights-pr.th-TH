---
title: ส่งออก eDiscovery/ผลลัพธ์การค้นหาเนื้อหา
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483735"
---
# <a name="export-ediscoverycontent-search-results"></a>ส่งออก eDiscovery/ผลลัพธ์การค้นหาเนื้อหา

คุณอาจต้องส่งออกผลลัพธ์การค้นหาของคุณเป็นไฟล์ PST (จากอีเมล) หรือไปยังเอกสาร Office ดั้งเดิม (จากไซต์ SharePoint และ OneDrive for Business) ถ้าเป็นเช่น นี้ ให้ทต่อไปนี้:

- ตรวจสอบให้แน่ใจว่าบัญชีของคุณได้รับมอบหมายสิทธิ์ที่เหมาะสมในการส่งออก For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).
- ตรวจสอบให้แน่ใจว่าคอมพิวเตอร์ของคุณตรงตามเงื่อนไข [เบื้องต้น](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin)ทั้งหมด เบราว์เซอร์บางรายการไม่ได้รับการสนับสนุน เช่น Chrome
- เมื่อต้องการส่งออกจากการค้นหาเนื้อหา: a. ไปที่ศูนย์ [&การปฏิบัติตาม](https://protection.office.com/contentsearch) นโยบาย **แล้วคลิก** ค้นหา **แล้วเลือกการค้นหา** เนื้อหา บนหน้า **การค้นหา** เนื้อหา ให้เลือกการค้นหาที่บันทึกไว้
    b. บนบานหน้าต่างรายละเอียด ภายใต้ **ส่งออกผลลัพธ์ไปยังคอมพิวเตอร์** เลือก **เริ่ม** ส่งออก ถ้าคุณส่งออกกล่องจดหมายมากกว่า 100K คุณจะต้องใช้ PowerShell เพื่อดาวน์โหลดผลลัพธ์การส่งออก For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).

เมื่อต้องการเรียนรู้เพิ่มเติม [ให้ดู ส่งออกผลลัพธ์การค้นหา](https://go.microsoft.com/fwlink/?linkid=2102118)เนื้อหา