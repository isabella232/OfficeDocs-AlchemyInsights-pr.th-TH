---
title: รูปภาพผู้ใช้ยังคงปรากฏในแผนผังMicrosoft Teamsองค์กร
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422316"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>รูปภาพผู้ใช้ยังคงปรากฏในแผนผังMicrosoft Teamsองค์กร

ถ้าบุคคลอย่างน้อยหนึ่งรายในองค์กรของคุณถูกปิดใช้งานหรือถูกเอาออก และรูปภาพโปรไฟล์ของพวกเขายังคงปรากฏในแผนผังองค์กร อาจเป็นไปได้ว่าการตั้งค่า **ShowInAddressLists** ถูกตั้งค่าเป็น False: 

1. ไปที่ ศูนย์การจัดการ Microsoft 365 >[ผู้ใช้](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)ที่ใช้งานอยู่ แล้วเลือกผู้ใช้ที่มีรูปถ่ายที่ยังคงปรากฏขึ้น 
1. เลือก **แท็บ** จดหมาย และตรวจสอบให้แน่ใจว่า **แสดงในสมุดรายชื่อส่วนกลาง** ถูกตั้งค่า **เป็น** ไม่

ถ้าการตั้งค่า **ShowInAddressLists** **เป็น** ไม่ ใช้งานไม่ได้ ให้ตรวจสอบดังต่อไปนี้: 

- ผู้ใช้อาจแสดงจากรายการผู้รับในExchangeผู้รับ ดูข้อมูลเพิ่มเติมได้ที่ จัดการ[รายการที่อยู่ในExchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- ผู้ใช้อาจแสดงจากรายการที่อยู่ในAzure Active Directoryของคุณ ดูข้อมูลเพิ่มเติมได้ที่[Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 