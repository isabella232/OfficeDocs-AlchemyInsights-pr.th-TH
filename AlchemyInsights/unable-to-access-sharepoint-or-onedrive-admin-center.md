---
title: ไม่สามารถเข้าถึง SharePoint หรือศูนย์การจัดการ OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 627a4ef2900a6b9bbef7eb3f3a214ee7c371e354
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716474"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>ไม่สามารถเข้าถึง SharePoint หรือศูนย์การจัดการ OneDrive

- ถ้าไซต์ศูนย์การดูแล SharePoint หรือ OneDrive ของคุณไม่สามารถเข้าถึงหรือไม่พร้อมใช้งาน อาจมีปัญหาการบริการชั่วคราวที่ผู้ใช้พบความล่าช้าเป็นระยะ ๆ หรือข้อผิดพลาดในการนําทางเมื่อเข้าถึงไซต์ SharePoint หรือเนื้อหาของ OneDrive ตรวจสอบ[แดชบอร์ดสถานภาพบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่

- ผู้ดูแลระบบส่วนกลางและ SharePoint ต้องได้รับมอบหมายสิทธิ์การใช้งาน SharePoint บัญชีที่สร้างขึ้นใหม่เพิ่งได้รับมอบหมายด้วยบทบาทสิทธิ์การใช้งาน SharePoint หรือผู้ดูแลระบบอาจประสบปัญหาในการเข้าถึง SharePoint เช่น "การเข้าถึงถูกปฏิเสธ" หรือ "ไม่พบผู้ใช้" โปรดให้อย่างน้อย 24 ชั่วโมงสําหรับการซิงค์เพื่อให้เสร็จสมบูรณ์ในระบบของเรา เราเข้าใจว่า 24 ชั่วโมงอาจดูเหมือนเป็นเวลานาน ในหลายกรณีเรากําลังทํางานอยู่แล้วในการแก้ปัญหา

- ผู้ใช้การจัดการข้อมูลเฉพาะตัวที่มีสิทธิ์ ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) อาจได้รับการปฏิเสธการเข้าถึงถ้าหน้าต่างเวลาการเข้าถึงที่ได้รับอนุญาตมีขนาดเล็กมาก ให้ดูที่[การเข้าถึงถูกปฏิเสธไปยังบัญชี PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)