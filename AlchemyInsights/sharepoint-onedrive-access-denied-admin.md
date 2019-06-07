---
title: การแก้ไขปัญหาข้อความที่มีการเข้าถึงถูกปฏิเสธ
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760359"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความในศูนย์กลางการดูแล Sharepoint/OneDrive

หากคุณได้รับการเข้าถึงถูกปฏิเสธข้อความเมื่อคุณพยายามเรียกดูไปยังศูนย์ดูแล Sharepoint/OneDrive โปรดตรวจสอบให้แน่ใจว่าคุณ[มอบหมายสิทธิ์ให้กับผู้ใช้](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One) ถ้าผู้ใช้มีสิทธิ์การใช้งาน คุณควรทำแน่ใจว่า[กำหนดบทบาทเป็นผู้ดูแลระบบ](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)ที่สามารถเข้าถึงศูนย์การดูแลด้วย

ปัญหานี้สามารถเกิดขึ้นเมื่อผู้ใช้ถูกลบออก และสร้างขึ้นใหม่ ด้วยชื่อเดียวกันผู้ใช้หลัก (UPN) สร้างบัญชีใหม่ โดยใช้ค่า PUID (ID เฉพาะของ Passport) แตกต่างกัน เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขา ผู้ใช้มี PUID ที่ไม่ถูกต้อง สถานการณ์สมมติที่สองเกี่ยวข้องกับไดเรกทอรีการซิงโครไนส์กับ Active Directory หน่วยองค์กร (OU) ถ้าผู้ใช้มีอยู่แล้วลงชื่อเข้าใช้ SharePoint แล้วจะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้

เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนต่าง ๆ ในบทความ[การคืนค่าผู้ใช้ใน Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)

หมายเหตุ: ถ้าไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่มีการเข้าถึงไว้ก่อนหน้านี้ เป็นศูนย์ OneDrive หรือผู้ดูแลระบบ SharePoint อาจมีปัญหาการบริการชั่วคราว  [ตรวจสอบแดชบอร์ความสมบูรณ์ของการบริการ](https://portal.office.com/adminportal/home#/servicehealth)


