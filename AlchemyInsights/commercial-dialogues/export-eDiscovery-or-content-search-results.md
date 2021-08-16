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
ms.openlocfilehash: de5d6f2bbf32ca1b7a0bbb9dd416fb19186d2e72ad57fbf25d9b55bd733fdc21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988203"
---
# <a name="export-ediscoverycontent-search-results"></a>ส่งออก eDiscovery/ผลลัพธ์การค้นหาเนื้อหา

คุณอาจต้องส่งออกผลลัพธ์การค้นหาเป็นไฟล์ PST (จากอีเมล) หรือส่งออกไปยังเอกสารOffice (จากSharePoint OneDrive for Businessไซต์ของคุณ) ถ้าเป็นดังนั้น ให้ต่อไปนี้:

- ตรวจสอบให้แน่ใจว่าบัญชีผู้ใช้ของคุณได้รับการมอบหมายสิทธิ์ที่เหมาะสมเพื่อส่งออก For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).
- ตรวจสอบให้แน่ใจว่าคอมพิวเตอร์ของคุณตรงตามเงื่อนไข [เบื้องต้น](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin)ทั้งหมด บางเบราว์เซอร์ไม่ได้รับการสนับสนุน เช่น Chrome
- เมื่อต้องการส่งออกจากการค้นหาเนื้อหา: a. ไปที่ ศูนย์ [การรักษา&การปฏิบัติตาม](https://protection.office.com/contentsearch) นโยบาย **แล้วคลิก** ค้นหา **แล้วเลือก การค้นหา** เนื้อหา บนหน้า **การค้นหา** เนื้อหา ให้เลือกการค้นหาที่บันทึกไว้
    b. บนบานหน้าต่าง รายละเอียด ภายใต้ **ส่งออกผลลัพธ์ไปยัง** คอมพิวเตอร์ **เลือก เริ่ม** ส่งออก ถ้าคุณส่งออกกล่องจดหมายมากกว่า 100K คุณจะต้องใช้ PowerShell เพื่อดาวน์โหลดผลลัพธ์การส่งออก ดูข้อมูลเพิ่มเติมได้ที่ การส่งออก[ผลลัพธ์จากกล่องจดหมายมากกว่า 100K](https://go.microsoft.com/fwlink/?linkid=2143861)

เมื่อต้องการเรียนรู้เพิ่มเติม [ให้ดู ส่งออกผลลัพธ์การค้นหา](https://go.microsoft.com/fwlink/?linkid=2102118)เนื้อหา