---
title: เพิ่มกลุ่มลงในSharePointไซต์
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 52f3bca7e92e9523838b5ad691f8accf0e7d0d03df79bb575f93b024e32cf3c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093820"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>ปัญหาทั่วไปเมื่อสร้างไซต์ที่เชื่อมต่อกลุ่มในSharePoint

1. ถ้าคุณลบกลุ่มและไซต์ที่เชื่อมต่อและต้องการสร้างไซต์อื่นด้วย URL เดียวกัน คุณจะต้องเอาไซต์ก่อนหน้าออกอย่างถาวร

   - ดาวน์โหลด [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](/powershell/module/sharepoint-online/remove-sposite).
   - เอาไซต์ออกจากไซต์ที่ถูกลบโดยใช้ [cmdlet Remove-SPODeletedSite](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell Powershell is required to permanently delete group sites.

1. ถ้าคุณสร้างไซต์ที่เชื่อมต่อกับกลุ่มและรับคําเตือน:**มี** กลุ่มอื่นที่มีนามแฝงเดียวกันอยู่แล้ว ให้ตรวจสอบกลุ่มที่มีอยู่ศูนย์การจัดการ Microsoft 365 [](https://admin.microsoft.com/AdminPortal/Home#/groups) เมื่อต้องการแก้ไขปัญหา ให้ลบกลุ่มที่มีอยู่ถ้าไม่ต้องใช้อีกต่อไปหรือสร้างไซต์ด้วยการมอบหมายนามแฝงอื่น

1. มีหลายวิธีในการสร้างและใช้กลุ่มสมัยใหม่ด้วยSharePointหลากหลาย

   - คุณสามารถเชื่อมต่อไซต์ที่มีอยู่กับMicrosoft 365อื่นได้ ดูข้อมูลเพิ่มเติมได้ที่ เชื่อมต่อ[กลุ่มMicrosoft 365โดยใช้SharePointหลัก](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - เมื่อต้องการMicrosoft 365ไซต์ที่เชื่อมต่อกลุ่มคุณจะต้องสร้าง[ไซต์](https://admin.microsoft.com/sharepoint)ทีม
