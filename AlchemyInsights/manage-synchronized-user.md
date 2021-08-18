---
title: จัดการผู้ใช้ที่ซิงโครไนซ์
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114803"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>ไม่สามารถตั้งค่าที่อยู่อีเมลหลัก เปลี่ยนแอตทริบิวต์ของผู้ใช้ หรือลบผู้ใช้ที่ถูกซิงโครไนซ์

ถ้าเปิดใช้งานการซิงโครไนซ์ไดเรกทอรีกับสภาพแวดล้อมของคุณ แอตทริบิวต์ผู้ใช้หรือวัตถุบางอย่างจะไม่สามารถเปลี่ยนแปลงได้โดยใช้ศูนย์การจัดการ Microsoft 365

เมื่อต้องการจัดการผู้ใช้ที่ซิงโครไนซ์และแอตทริบิวต์ทั้งหมดให้สมบูรณ์ ให้ใช้ผู้ใช้ไดเรกทอรีที่ใช้งานอยู่ภายในเครื่องและคอนโซลการจัดการกลุ่ม (adsiedit.msc)  

อีกวิธีหนึ่งคือ คุณสามารถเปลี่ยนผู้ใช้แต่ละรายหรือแอตทริบิวต์ของผู้ใช้ที่ซิงโครไนซ์โดยใช้ Powershell เช่นที่แสดงในตัวอย่างทั่วไปเหล่านี้:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
