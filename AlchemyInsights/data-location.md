---
title: ตำแหน่งของข้อมูล
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
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627865"
---
# <a name="data-location"></a>ตำแหน่งของข้อมูล

คุณสามารถดูตำแหน่งที่ตั้งของผู้เช่า Office ๓๖๕ของคุณในศูนย์การจัดการหรือโดยการเชื่อมต่อกับ Exchange แบบออนไลน์ผ่านทาง PowerShell


**ศูนย์การจัดการ:**
1. ล็อกอินเข้าสู่[ศูนย์กลางการดูแล](https://admin.microsoft.com/Adminportal/Home)ระบบ
2. เลือก**โปรไฟล์องค์กร****การตั้งค่า** > 
3. ภายใต้**ตำแหน่งข้อมูล**ให้เลือก**ดูรายละเอียด**


**Powershell:**
1. เชื่อมต่อกับการแลกเปลี่ยนแบบออนไลน์โดยใช้ Windows PowerShell
2. ดำเนินการ cmdlet การ[รับองค์กร](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit)เพื่อแสดงรายการของคุณสมบัติของผู้เช่าของคุณ 
3. มองไปที่คุณสมบัติองค์กร

เมื่อคุณมีตำแหน่งข้อมูลสำหรับ EXO และที่คุณสามารถกำหนดตำแหน่งข้อมูลสำหรับบริการอื่นๆที่คุณอาจใช้จาก[ตำแหน่งที่ข้อมูลของคุณอยู่](https://products.office.com/where-is-your-data-located)