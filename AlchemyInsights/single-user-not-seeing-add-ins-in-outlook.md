---
title: ผู้ใช้คนเดียวไม่เห็น add-in ใน Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719684"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>ผู้ใช้คนเดียวไม่เห็น add-in ใน Outlook

ผู้ใช้อาจเป็นส่วนหนึ่งของบทบาทที่ไม่มีพารามิเตอร์ AppsForOfficeEnabled ที่ถูกต้อง เรียกใช้ cmdlet นี้เพื่อค้นหาว่าบทบาทที่ถูกต้องเกี่ยวข้องกับผู้ใช้:

Get-ManagementRoleAssignment-RoleAssignee user@domain.com-การมอบ $false รูปแบบ-ตาราง-บทบาทอัตโนมัติ, RoleAssigneeName, RoleAssigneeType

สำหรับข้อมูลเพิ่มเติมให้ดู [ที่ระบุผู้ดูแลระบบและผู้ใช้ที่สามารถติดตั้งและจัดการ add-in สำหรับ Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)ได้
