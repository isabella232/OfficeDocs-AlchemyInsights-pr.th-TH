---
title: ตําแหน่งที่ตั้งข้อมูล
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655301"
---
# <a name="data-location"></a>ตําแหน่งที่ตั้งข้อมูล

คุณสามารถดูตําแหน่งที่ตั้งของผู้เช่าของคุณในศูนย์การจัดการ หรือโดยการเชื่อมต่อกับ Exchange Online ผ่านทาง PowerShell


**ศูนย์การจัดการ:**
1. เข้าสู่ระบบ[ที่ ศูนย์การจัดการ](https://admin.microsoft.com/Adminportal/Home)
2. เลือก**โปรไฟล์องค์กร****การตั้งค่า** > 
3. ภายใต้**ตําแหน่งที่ตั้งข้อมูล****ให้เลือก**


**Powershell:**
1. เชื่อมต่อกับการแลกเปลี่ยนแบบออนไลน์ โดยใช้ Windows PowerShell
2. ดําเนินการ cmdlet[รับ OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit)เพื่อแสดงรายการของคุณสมบัติของผู้เช่า 
3. ดูที่คุณสมบัติรหัสองค์กร

เมื่อคุณมีตําแหน่งข้อมูลสําหรับ EXO และ SPO คุณสามารถกําหนดตําแหน่งข้อมูลสําหรับบริการอื่น ๆ ที่คุณอาจใช้จาก[ตําแหน่งข้อมูลของคุณอยู่](https://products.office.com/where-is-your-data-located)