---
title: เพิ่มกลุ่มไปยังไซต์ SharePoint
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
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: d1aad215f8aa636ba89c93a13a0c9d90e997f752
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/06/2020
ms.locfileid: "44064412"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>ปัญหาเมื่อสร้างไซต์ที่เชื่อมโยงกลุ่มใน SharePoint

1. พบปัญหาทั่วไปเมื่อสร้างหรือสร้างไซต์ที่เชื่อมโยงกลุ่มใหม่
หากคุณลบกลุ่มและไซต์ที่เชื่อมโยงแล้วและต้องการสร้างไซต์อื่นที่มี URL เดียวกัน คุณจะต้องนําไซต์ก่อนหน้าออกอย่างถาวร

   - ดาวน์โหลด[เชลล์การจัดการ SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการเริ่มต้นใช้งาน Powershell ให้ดูที่[การเริ่มต้นใช้งานเชลล์การจัดการ SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - เอาไซต์จากไซต์ที่ถูกลบโดยใช้ cmdlet[ลบ SPODeleted ไซต์](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)Powershell Powershell จําเป็นในการลบไซต์กลุ่มอย่างถาวร

1. ถ้าคุณกําลังสร้างไซต์ที่เชื่อมต่อกลุ่มและได้รับคําเตือน:**มีอีกกลุ่มหนึ่งที่มีนามแฝงเดียวกันอยู่แล้ว**ให้ตรวจสอบกลุ่มที่มีอยู่จาก[ศูนย์การจัดการ Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups) หากต้องการแก้ปัญหานี้ ให้ลบกลุ่มที่มีอยู่หากไม่จําเป็นหรือสร้างไซต์ที่มีการกําหนดนามแฝงอื่น

1. มีวิธีการสร้างและใช้กลุ่มสมัยใหม่กับ SharePoint หลายวิธี

   - คุณสามารถเชื่อมต่อไซต์ที่มีอยู่กับกลุ่ม Microsoft 365 ได้ สําหรับข้อมูลเพิ่มเติม ให้ดูที่[เชื่อมต่อกลุ่ม Microsoft 365 โดยใช้ส่วนติดต่อผู้ใช้ของ SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - เมื่อต้องการสร้างไซต์ที่เชื่อมโยงกลุ่ม Microsoft 365 คุณจะต้องสร้าง[ไซต์ทีม](https://admin.microsoft.com/sharepoint)
