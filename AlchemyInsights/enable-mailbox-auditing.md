---
title: เปิดใช้งานการตรวจสอบกล่องจดหมาย
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806310"
---
# <a name="enable-mailbox-auditing"></a>เปิดใช้งานการตรวจสอบกล่องจดหมาย

เมื่อต้องการเปิดใช้งานการตรวจสอบกล่องจดหมายสำหรับผู้ใช้คนเดียวหรือทั้งองค์กรจะต้องเรียกใช้ cmdlet ต่อไปนี้จาก Shell Power ระยะไกล:
  
 **ผู้ใช้คนเดียว**
  
ตั้งค่ากล่องจดหมาย-ข้อมูลประจำตัว "Jane AuditEnabled $true
  
 **องค์กร**
  
กล่องจดหมาย-ResultSize ไม่จำกัด-ตัวกรอง {RecipientTypeDetails-eq "UserMailbox"} | ตั้งค่ากล่องจดหมาย-$true AuditEnabled
  
[ศึกษาเพิ่มเติม](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

