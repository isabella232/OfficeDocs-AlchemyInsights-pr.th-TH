---
title: ผู้ใช้หลายคนได้รับข้อผิดพลาดการเข้าถึงถูกปฏิเสธในขณะที่เพิ่ม Add-in Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 5e5f881ad72d2a0f76c8659d6b1044bf6a18464fa8d65c079e44eb1a2afd4431
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065411"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>ผู้ใช้หลายคนได้รับข้อผิดพลาดการเข้าถึงถูกปฏิเสธในขณะที่เพิ่ม Add-in Outlook

คุณสามารถระบุได้ว่าผู้ดูแลระบบใดในองค์กรของคุณที่มีสิทธิ์ในการติดตั้งและจัดการ Add-in Outlook คุณยังสามารถระบุผู้ใช้ในองค์กรของคุณที่มีสิทธิ์ในการติดตั้งและจัดการ Add-in เพื่อใช้ของพวกเขาเองได้

For details, [see Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

เมื่อต้องการตรวจสอบว่าคุณได้มอบหมายสิทธิ์ให้กับผู้ใช้เรียบร้อยแล้ว หรือไม่ ให้แทนที่ด้วยชื่อของบทบาทเพื่อตรวจสอบ และเรียกใช้สั่งต่อไปนี้ใน Exchange Online <Role Name> PowerShell:

Get-ManagementRoleAssignment -Role " <Role Name> " -GetSffectiveUsers

ตัวอย่างนี้แสดงวิธีการตรวจสอบว่าคุณได้มอบหมายสิทธิ์ให้ติดตั้ง Add-in จาก Office Store ให้กับองค์กรหรือไม่

PowerShell

-Role "Org Marketplace Apps" -GetSffectiveUsers

ในผลลัพธ์ Get-ManagementRoleAssignment ให้รีวิวรายการในคอลัมน์ Effective Users

For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 