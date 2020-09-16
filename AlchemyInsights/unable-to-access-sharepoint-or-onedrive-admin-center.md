---
title: ไม่สามารถเข้าถึงศูนย์การจัดการ SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: a70b0708b325c5feaefec3d97c957086d7f62cc6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749497"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>ไม่สามารถเข้าถึงศูนย์การจัดการ SharePoint หรือ OneDrive

- ถ้าไซต์ SharePoint หรือศูนย์การจัดการ OneDrive ของคุณไม่สามารถเข้าถึงได้หรือไม่พร้อมใช้งานอาจมีปัญหาด้านบริการชั่วคราวที่ผู้ใช้พบความล่าช้าหรือข้อผิดพลาดในการนำทางเมื่อเข้าถึงไซต์ SharePoint หรือเนื้อหา OneDrive ตรวจสอบ [แดชบอร์ดความสมบูรณ์ของบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่

- ผู้ดูแลระบบส่วนกลางและผู้ดูแลระบบ SharePoint จำเป็นต้องได้รับการกำหนดสิทธิ์การใช้งาน SharePoint บัญชีผู้ใช้ที่สร้างขึ้นใหม่เพิ่งมอบหมายให้กับสิทธิ์การใช้งาน SharePoint หรือบทบาทผู้ดูแลระบบอาจประสบปัญหาในการเข้าถึง SharePoint เช่น "access denied" หรือ "ไม่พบผู้ใช้" โปรดให้การซิงค์อย่างน้อย24ชั่วโมงเพื่อให้เสร็จสมบูรณ์ในระบบของเรา เราเข้าใจว่า24ชั่วโมงอาจดูเหมือนเป็นเวลานาน ในหลายกรณีเรากำลังทำงานกับโซลูชันอยู่แล้ว

- ผู้ใช้ที่มีสิทธิ์ในการจัดการข้อมูลประจำตัว ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) อาจได้รับการเข้าถึงถูกปฏิเสธถ้าหน้าต่างเวลาการเข้าถึงที่อนุญาตมีขนาดเล็กมากให้ดู[การเข้าถึงถูกปฏิเสธไปยังบัญชีผู้ใช้ PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)