---
title: รายงานใน ศูนย์การจัดการ Microsoft 365ไม่แสดงชื่อผู้ใช้ที่สามารถอ่านได้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327833"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>รายงานใน ศูนย์การจัดการ Microsoft 365ไม่แสดงชื่อผู้ใช้ที่สามารถอ่านได้

รายงานใน ศูนย์การจัดการ Microsoft 365ไม่แสดงชื่อผู้ใช้ แต่แสดงค่าตัวเลขพยชนะผสมตัวเลข เช่น B2BC6C15BB9FCDEA71Y5CD302D228CC8 แทน

นี่คือลักษณะการเหล่านี้และได้รับการติดต่อสื่อสารในศูนย์ข้อความ (MC275344 ที่เผยแพร่เมื่อวันที่ 3 ส.ค. 2021) 

ผู้ดูแลระบบส่วนกลางสามารถแปลงการเปลี่ยนแปลงนี้ให้กับผู้เช่าของตนและแสดงข้อมูลผู้ใช้ที่ระบุตัวตนได้ ถ้าข้อปฏิบัติด้านความเป็นส่วนตัวขององค์กรอนุญาต เมื่อต้องการแปลงการเปลี่ยนแปลงของผู้เช่า:

1. ในศูนย์การจัดการ ให้ไปที่ **การตั้งค่า**  >  **Org**  >  [**Settings Services**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services )**แล้วเลือก** รายงาน 
1. **ภายใต้ เลือกวิธีแสดงข้อมูล** ผู้ใช้ ให้เลือก **แสดงข้อมูลผู้ใช้** ที่ระบุได้ในรายงาน แล้วเรียกใช้รายงานอีกครั้ง