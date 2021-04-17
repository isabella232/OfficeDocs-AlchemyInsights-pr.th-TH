---
title: ไม่สามารถเข้าถึงศูนย์การจัดการ SharePoint หรือ OneDrive ได้
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824454"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>ไม่สามารถเข้าถึงศูนย์การจัดการ SharePoint หรือ OneDrive ได้

- ถ้าไซต์ศูนย์การจัดการ SharePoint หรือ OneDrive ของคุณไม่สามารถเข้าถึงได้หรือไม่พร้อมใช้งาน อาจมีปัญหาชั่วคราวที่ผู้ใช้พบความล่าช้าหรือการนําทางที่ผิดพลาดเป็นระยะๆ เมื่อเข้าถึงไซต์ SharePoint หรือเนื้อหา OneDrive ตรวจสอบ [แดชบอร์ดสถานภาพ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) บริการเพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่

- ผู้ดูแลระบบส่วนกลางและผู้ดูแลระบบ SharePoint ต้องได้รับการมอบหมายสิทธิ์การใช้งาน SharePoint บัญชีที่สร้างขึ้นใหม่ที่เพิ่งมอบหมายด้วยสิทธิ์การใช้งาน SharePoint หรือบทบาทผู้ดูแลระบบอาจพบปัญหาในการเข้าถึง SharePoint เช่น "การเข้าถึงถูกปฏิเสธ" หรือ "ไม่พบผู้ใช้" โปรดให้เวลาอย่างน้อย 24 ชั่วโมงเพื่อให้การซิงค์เสร็จสมบูรณ์ระหว่างระบบของเรา เราเข้าใจว่าเวลา 24 ชั่วโมงอาจดูเป็นเวลานาน ในหลายกรณี เราแก้ไขปัญหาเรียบร้อยแล้ว

- ผู้ใช้การจัดการข้อมูลเฉพาะตัวที่ได้รับ[สิทธิ์ (PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)อาจถูกปฏิเสธการเข้าถึงถ้าหน้าต่างเวลาการเข้าถึงที่อนุญาตมีขนาดเล็กมาก ให้ดู[การเข้าถึงถูกปฏิเสธบัญชี PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)