---
title: การเพิ่มกลุ่มให้กับไซต์ SharePoint
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
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770370"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>ปัญหาเมื่อสร้างไซต์ที่เชื่อมต่อกับกลุ่มใน SharePoint

1. ปัญหาทั่วไปบางอย่างที่พบเมื่อสร้างหรือสร้างไซต์ที่เชื่อมต่อกับกลุ่มอีกครั้ง
หากคุณลบกลุ่มและไซต์ที่เชื่อมต่อและต้องการสร้างไซต์อื่นด้วย URL เดียวกันคุณจะต้องลบไซต์ก่อนหน้านี้อย่างถาวร

   - ดาวน์โหลด[เชลล์การจัดการ SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเริ่มต้นใช้งาน Powershell ให้ดู[ที่การเริ่มต้นใช้งานเชลล์จัดการแบบออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - เอาไซต์ออกจากไซต์ที่ถูกลบโดยใช้ cmdlet Powershell[ลบ SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) จำเป็นต้องมี Powershell เพื่อลบไซต์กลุ่มอย่างถาวร

1. ถ้าคุณกำลังสร้างไซต์ที่เชื่อมต่อกับกลุ่มและได้รับคำเตือน:**กลุ่มอื่นที่มีนามแฝงเดียวกันอยู่แล้ว**ให้ตรวจสอบกลุ่มที่มีอยู่จาก[Office ๓๖๕จากศูนย์ดูแล](https://admin.microsoft.com/AdminPortal/Home#/groups) เมื่อต้องการแก้ไขปัญหานี้ให้ลบกลุ่มที่มีอยู่ถ้าไม่จำเป็นหรือสร้างไซต์ด้วยนามแฝงที่แตกต่างกันที่กำหนดไว้

1. มีหลายวิธีในการสร้างและใช้กลุ่มที่ทันสมัยกับ SharePoint

   - คุณสามารถเชื่อมต่อไซต์ที่มีอยู่ไปยังกลุ่ม Office ๓๖๕ สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การเชื่อมต่อกลุ่ม Office ๓๖๕โดยใช้ส่วนติดต่อผู้ใช้ของ SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - เมื่อต้องการสร้างไซต์ที่เชื่อมต่อกับกลุ่ม Office ๓๖๕คุณจะต้องสร้าง[ไซต์ทีม](https://admin.microsoft.com/sharepoint)
