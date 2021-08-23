---
title: การควบคุมแอปไม่ใช้งานได้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12676"
ms.openlocfilehash: 661c2206fa51796c86e168af7c6ef6bf5e76092c
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454981"
---
# <a name="app-governance-is-not-working"></a>การควบคุมแอปไม่ใช้งานได้

การควบคุมแอปพร้อมใช้งานแล้วในการแสดงตัวอย่างสาธารณะ ถ้าคุณมีปัญหากับ การควบคุมแอป (ตัวอย่าง) ไม่ใช้งานได้ ให้ลองต่อไปนี้:

- เพื่อให้แน่ใจว่าคุณตรงตามเงื่อนไขเบื้องต้นทั้งหมด ให้ดูที่ [เริ่มต้นใช้งาน](https://docs.microsoft.com/microsoft-365/compliance/app-governance-get-started)ด่วน

- ให้ปฏิบัติตามขั้นตอนที่ต้องระบุเพื่อเปิดใช้งานรุ่นทดลองใช้ฟรี For details, see [Get started with app governance](https://docs.microsoft.com/microsoft-365/compliance/app-governance-get-started#add-app-governance-to-your-microsoft-365-account). 

    **หมายเหตุ**: การรวมเพียงการสลับMicrosoft Cloud App Security (MCAS) จะไม่เปิดใช้งานการควบคุมแอปเวอร์ชันทดลองใช้ฟรี คุณต้องปฏิบัติตามขั้นตอนการเปิดใช้งาน

- เมื่อต้องการเพิ่มการควบคุมแอปไปยังบานหน้าต่างนําทางด้านซ้ายของศูนย์การปฏิบัติตามนโยบาย ให้ไปที่ แค็ตตาล็อกโซลูชัน เพื่อเพิ่ม การควบคุมแอป การเปลี่ยนแปลงอาจใช้เวลาถึง 24 ชั่วโมงหลังจากลงทะเบียนเพื่อให้มีผล

- ตรวจสอบให้แน่ใจว่าคุณมีบทบาทที่เหมาะสมที่มอบหมายให้กับบัญชีของคุณ:

    1. ไปที่[ศูนย์การจัดการ Microsoft 365](https://admin.microsoft.com/Adminportal/Home#/users)บทบาทของคุณและดูบทบาทที่คุณได้รับมอบหมายโดยการเลือกชื่อของคุณและตรวจสอบบทบาทที่แสดงรายการอยู่ภายใต้ บทบาท ในบานหน้าต่างเมนูปลิว

    1. บนหน้า [เริ่มต้นใช้งานด่วน](https://aka.ms/appgovernancepreview) ให้ตรวจสอบว่าบทบาทของคุณเป็นหนึ่งในบทบาทที่มีสิทธิ์เข้าถึงการควบคุมแอป ดูบทบาทของผู้ดูแลระบบที่ยอมรับได้ [ให้ดู บทบาท](https://docs.microsoft.com/microsoft-365/compliance/app-governance-get-started#administrator-roles)ผู้ดูแลระบบ 

    1. ถ้าคุณไม่ได้ได้รับมอบหมายบทบาทที่เหมาะสม ให้ขอการมอบหมายบทบาทที่มีสิทธิ์จากผู้ดูแลระบบของคุณ

For more information on getting started with App Governance, see [Get started with app governance (in preview)](https://docs.microsoft.com/microsoft-365/compliance/app-governance-get-started).