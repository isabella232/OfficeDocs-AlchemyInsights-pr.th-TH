---
title: เพิ่มกลุ่มลงในไซต์ SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582830"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>ปัญหาเมื่อสร้างไซต์ที่เชื่อมต่อกลุ่มใน SharePoint

1. ปัญหาทั่วไปบางอย่างที่พบเมื่อสร้างหรือสร้างไซต์ที่เชื่อมต่อกลุ่มใหม่
ถ้าคุณลบกลุ่มและไซต์ที่เชื่อมต่อและต้องการสร้างไซต์อื่นที่มี URL เดียวกัน คุณจะต้องลบไซต์ก่อนหน้าอย่างถาวร

   - ดาวน์โหลด[เชลล์จัดการ SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการเริ่มต้นใช้ Powershell ให้ดูที่[การเริ่มต้นใช้งานเชลล์การจัดการแบบออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - เอาไซต์จากไซต์ที่ถูกลบโดยใช้ cmdlet ของ Powershell[ลบ SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) จําเป็นต้องมี Powershell เพื่อลบไซต์กลุ่มอย่างถาวร

1. ถ้าคุณกําลังสร้างไซต์ที่เชื่อมต่อกลุ่มและได้รับคําเตือน:**มีอีกกลุ่มหนึ่งที่มีนามแฝงเดียวกันอยู่แล้ว**ให้ตรวจสอบกลุ่มที่มีอยู่จาก[ศูนย์การจัดการ Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups) เมื่อต้องการแก้ปัญหา ให้ลบกลุ่มที่มีอยู่

1. มีวิธีต่างๆ ในการสร้างและใช้กลุ่มสมัยใหม่กับ SharePoint

   - คุณสามารถเชื่อมต่อไซต์ที่มีอยู่กับกลุ่ม Microsoft 365 สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การเชื่อมต่อกลุ่ม Microsoft 365 โดยใช้ส่วนติดต่อผู้ใช้ของ SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - เมื่อต้องการสร้างไซต์ที่เชื่อมต่อกลุ่ม Microsoft 365 คุณจะต้องสร้าง[ไซต์ทีม](https://admin.microsoft.com/sharepoint)
