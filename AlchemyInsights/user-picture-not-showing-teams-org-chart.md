---
title: รูปภาพผู้ใช้ไม่แสดงในMicrosoft Teamsองค์กรของคุณ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792888"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>รูปภาพผู้ใช้ไม่แสดงในMicrosoft Teamsองค์กรของคุณ

ถ้าบุคคลอย่างน้อยหนึ่งรายในองค์กรของคุณไม่มีรูปภาพโปรไฟล์ของพวกเขาในแผนผังองค์กร อาจเป็นไปได้ว่าการตั้งค่า **ShowInAddressLists** ถูกตั้งค่า **เป็น False**:

1. ไปที่ ศูนย์การจัดการ Microsoft 365 >[**ผู้ใช้**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)ที่ใช้งานอยู่ แล้วเลือกผู้ใช้ที่มีรูปถ่ายที่หายไป 
1. เลือก **แท็บ** จดหมาย และตรวจสอบให้แน่ใจว่า **แสดงในสมุดรายชื่อส่วนกลาง** ถูกตั้งค่า **เป็น** ใช่ 

ถ้าการตั้งค่า **ShowInAddressLists** **เป็น** ใช่ ไม่ได้ผล ให้ตรวจสอบดังต่อไปนี้:

- ผู้ใช้อาจถูกซ่อนจากรายชื่อผู้รับในExchangeของคุณ ดูข้อมูลเพิ่มเติมได้ที่ จัดการ[รายการที่อยู่ในExchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- ผู้ใช้อาจถูกซ่อนจากรายการที่อยู่ในAzure Active Directory ดูข้อมูลเพิ่มเติมได้ที่[Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 
