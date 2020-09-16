---
title: แก้ไขข้อความปฏิเสธการเข้าถึง
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767682"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>การแก้ไขปัญหาการเข้าถึงปฏิเสธข้อความในศูนย์การจัดการ Sharepoint/OneDrive

ถ้าคุณได้รับข้อความปฏิเสธการเข้าถึงเมื่อพยายามเรียกดูไปยังศูนย์การจัดการ Sharepoint/OneDrive โปรดตรวจสอบให้แน่ใจว่าคุณได้[กำหนดสิทธิ์การใช้งานให้กับผู้ใช้](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) ถ้าผู้ใช้มีสิทธิ์การใช้งานคุณควรตรวจสอบให้แน่ใจว่าผู้ใช้ได้รับ [มอบหมายบทบาทผู้ดูแลระบบ](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) ที่สามารถเข้าถึงศูนย์การจัดการได้

ปัญหานี้อาจเกิดขึ้นเมื่อผู้ใช้ถูกลบและสร้างขึ้นใหม่ด้วยชื่อผู้ใช้หลักเดียวกัน (UPN) บัญชีผู้ใช้ใหม่ถูกสร้างโดยใช้ค่า PUID (ID ที่ไม่ซ้ำกันของ Passport) ที่แตกต่างกัน เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขาผู้ใช้มี PUID ที่ไม่ถูกต้อง สถานการณ์สมมติที่สองจะเกี่ยวข้องกับการซิงโครไนซ์ไดเรกทอรีกับหน่วยองค์กร Active Directory (OU) ถ้าผู้ใช้ได้ลงชื่อเข้าใช้ SharePoint เรียบร้อยแล้วและจะถูกย้ายไปยัง OU และ resynced ที่แตกต่างกันกับ SharePoint พวกเขาอาจประสบปัญหานี้

เมื่อต้องการแก้ไขปัญหานี้คุณควรคืนค่า UPN ต้นฉบับที่มีขั้นตอนในบทความให้[คืนค่าผู้ใช้ใน Microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

หมายเหตุ: ถ้าศูนย์การจัดการ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่มีการเข้าถึงก่อนหน้านี้อาจมีปัญหาในการบริการชั่วคราว  [ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)


