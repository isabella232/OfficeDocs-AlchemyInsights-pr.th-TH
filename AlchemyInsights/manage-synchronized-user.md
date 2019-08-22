---
title: จัดการผู้ใช้ให้ตรงกัน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542036"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>ไม่สามารถกำหนดที่อยู่อีเมลหลัก หรือเปลี่ยนแอตทริบิวต์ของผู้ใช้

ถ้าเปิดใช้งานการซิงโครไนส์ของไดเรกทอรีสำหรับสภาพแวดล้อมของคุณ บางแอตทริบิวต์ผู้ใช้หรือวัตถุที่ไม่สามารถเปลี่ยนใช้ Microsoft 365 admin ศูนย์

เมื่อต้องการจัดการผู้ใช้ให้ตรงกันและคุณลักษณะทั้งหมดของทั้งหมด ใช้ของไดเรกทอรีที่ใช้งานอยู่ภายในเครื่องผู้ใช้และกลุ่มคอนโซลการจัดการ (adsiedit.msc)  

อีกวิธีหนึ่งคือ คุณสามารถเปลี่ยนแปลงแต่ละคนหรือแอตทริบิวต์สำหรับผู้ใช้ให้ตรงกันโดยใช้ powershell ที่แสดงในตัวอย่างเหล่านี้ทั่วไปเช่น: 
- การ user2@yourvanitydomain.onmicrosoft.com - AlternateEmailAddresses user@yourdomain.onmicrosoft.com - UserPrincipalName ชุด MsolUser
- ชุด-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "ผู้ใช้ทดสอบ" - เขตข้อมูล LastName "ผู้ใช้" - "ผู้จัดการ" ชื่อเรื่อง-แผนก "ทรัพยากรบุคคล"
- เอา-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com