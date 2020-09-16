---
title: เพิ่มกลุ่มลงในไซต์ SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771227"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>ปัญหาเมื่อสร้างไซต์ที่เชื่อมต่อกับกลุ่มใน SharePoint

1. ปัญหาทั่วไปบางอย่างที่พบเมื่อสร้างหรือสร้างไซต์ที่เชื่อมต่อกับกลุ่มอีกครั้ง
ถ้าคุณลบกลุ่มและไซต์ที่เชื่อมต่อและต้องการสร้างไซต์อื่นที่มี URL เดียวกันคุณจำเป็นต้องเอาไซต์ก่อนหน้าออกอย่างถาวร

   - ดาวน์โหลด [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเริ่มต้นใช้งาน Powershell ให้ดู[ที่การเริ่มต้นใช้งาน SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - เอาไซต์ออกจากไซต์ที่ถูกลบโดยใช้ cmdlet Powershell[เอา SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) จำเป็นต้องใช้ Powershell เพื่อลบไซต์กลุ่มอย่างถาวร

1. ถ้าคุณกำลังสร้างไซต์ที่เชื่อมต่อกับกลุ่มและได้รับคำเตือน:**กลุ่มอื่นที่มีนามแฝงเดียวกันอยู่แล้ว**ให้ตรวจสอบกลุ่มที่มีอยู่จาก[ศูนย์การจัดการ Microsoft ๓๖๕](https://admin.microsoft.com/AdminPortal/Home#/groups) เมื่อต้องการแก้ไขปัญหานี้ให้ลบกลุ่มที่มีอยู่ถ้าไม่จำเป็นต้องใช้อีกต่อไปหรือสร้างไซต์ด้วยนามแฝงอื่นที่มอบหมาย

1. มีหลายวิธีในการสร้างและใช้กลุ่มที่ทันสมัยกับ SharePoint

   - คุณสามารถเชื่อมต่อไซต์ที่มีอยู่ไปยังกลุ่ม Microsoft ๓๖๕ สำหรับข้อมูลเพิ่มเติมให้ดู[ที่เชื่อมต่อกลุ่ม Microsoft ๓๖๕โดยใช้ส่วนติดต่อผู้ใช้ของ SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - เมื่อต้องการสร้างไซต์ Microsoft ๓๖๕กลุ่มที่เชื่อมต่ออยู่คุณจำเป็นต้องสร้าง[ไซต์ทีม](https://admin.microsoft.com/sharepoint)
