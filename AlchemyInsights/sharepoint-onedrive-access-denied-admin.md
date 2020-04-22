---
title: การแก้ไขปัญหาข้อความปฏิเสธการเข้าถึง
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758539"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความในศูนย์การจัดการ Sharepoint/OneDrive

ถ้าคุณได้รับการเข้าถึงถูกปฏิเสธข้อความเมื่อพยายามที่จะเรียกดูไปยังศูนย์การจัดการ Sharepoint/OneDrive โปรดตรวจสอบให้แน่ใจว่า คุณ[กําหนดสิทธิ์การใช้งานให้กับผู้ใช้](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One) ถ้าผู้ใช้มีสิทธิ์การใช้งาน คุณควรตรวจสอบให้แน่ใจว่าผู้ใช้ได้รับ[มอบหมายบทบาทผู้ดูแลระบบ](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)ที่สามารถเข้าถึงศูนย์การจัดการได้

ปัญหานี้อาจเกิดขึ้นได้เมื่อผู้ใช้ถูกลบ และสร้างใหม่ ด้วยชื่อหลัก (UPN) เดียวกัน บัญชีใหม่ถูกสร้างขึ้น โดยใช้ค่า PUID (รหัสเฉพาะของ Passport) ที่แตกต่างกัน เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของตนเอง สถานการณ์สมมติที่สองเกี่ยวข้องกับการซิงโครไนส์ของไดเรกทอรีกับ Active Directory องค์กรหน่วย (OU) ถ้าผู้ใช้ได้ลงชื่อเข้าใช้ SharePoint แล้ว จะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้

เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนต่างๆ ในบทความ[คืนค่าผู้ใช้ใน Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)

หมายเหตุ: ถ้าศูนย์การจัดการ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสําหรับผู้ใช้หลายคนที่เคยมีการเข้าถึง อาจมีปัญหาการบริการชั่วคราว  [ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)


