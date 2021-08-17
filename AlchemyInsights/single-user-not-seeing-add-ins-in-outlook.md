---
title: ผู้ใช้คนเดียวไม่เห็น Add-in ในOutlook
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
ms.openlocfilehash: 647a17bb5220d3591934c4f53cf417d42810b2c1a681bafd3e2d703abbfcbc64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050677"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>ผู้ใช้คนเดียวไม่เห็น Add-in ในOutlook

ผู้ใช้อาจเป็นส่วนหนึ่งของบทบาทที่ไม่มีพารามิเตอร์ AppsForOfficeEnabled ที่ถูกต้อง เรียกใช้ cmdlet นี้เพื่อดูว่าบทบาทที่ถูกต้องเชื่อมโยงกับผู้ใช้หรือไม่:

Get-ManagementRoleAssignment -roleAssignee user@domain.com -การมอบหมาย$false | Format-Table -บทบาทอัตโนมัติ,RoleAssigneeName,RoleAssigneeType

For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
