---
title: ไม่สามารถเข้าถึงศูนย์การจัดการSharePointหรือOneDriveได้
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
ms.openlocfilehash: afb28ccae2c9f087f1e1417cb6594cedc908e1cf759a5d1e6d92c4ee9a75527d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020463"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>ไม่สามารถเข้าถึงศูนย์การจัดการSharePointหรือOneDriveได้

- ถ้าไซต์ศูนย์การจัดการ SharePoint หรือ OneDrive ของคุณไม่สามารถเข้าถึงได้หรือไม่พร้อมใช้งาน อาจเป็นปัญหาบริการชั่วคราวที่ผู้ใช้พบความล่าช้าหรือการนําทางที่ผิดพลาดเป็นระยะเมื่อเข้าถึงไซต์ SharePoint หรือเนื้อหา OneDrive ตรวจสอบ [แดชบอร์ดสถานภาพ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) บริการเพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่

- ผู้ดูแลระบบส่วนกลางSharePointและผู้ดูแลระบบต้องได้รับการSharePointสิทธิ์การใช้งานของคุณ บัญชีที่สร้างขึ้นใหม่ที่เพิ่งมอบหมายด้วยสิทธิ์การใช้งาน SharePointหรือบทบาทผู้ดูแลระบบอาจพบปัญหาในการเข้าถึงSharePoint เช่น "การเข้าถึงถูกปฏิเสธ" หรือ "ไม่พบผู้ใช้" โปรดให้เวลาอย่างน้อย 24 ชั่วโมงเพื่อให้การซิงค์เสร็จสมบูรณ์ระหว่างระบบของเรา เราเข้าใจว่าเวลา 24 ชั่วโมงอาจดูเป็นเวลานาน ในหลายกรณี เราแก้ไขปัญหาเรียบร้อยแล้ว

- Privileged Identity Management[( PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) ผู้ใช้อาจได้รับการเข้าถึงถูกปฏิเสธถ้าหน้าต่างเวลาการเข้าถึงที่อนุญาตมีขนาดเล็กมาก ให้ดู[การเข้าถึงถูกปฏิเสธบัญชี PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)