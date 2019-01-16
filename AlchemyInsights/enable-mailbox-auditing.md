---
title: เปิดใช้งานการตรวจสอบของกล่องจดหมาย
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28315989"
---
# <a name="enable-mailbox-auditing"></a>เปิดใช้งานการตรวจสอบของกล่องจดหมาย

เมื่อต้องการเปิดใช้งานการตรวจสอบของกล่องจดหมายสำหรับผู้ใช้คนเดียวหรือทั้งองค์กร ต้องรันการ cmdlet ของต่อไปนี้จากเชลล์พลังงานระยะไกล:
  
 **ผู้ใช้คนเดียว**
  
ตั้งค่าจดหมาย - รหัสประจำตัว "เจนด" - AuditEnabled $true
  
 **องค์กร**
  
รับจดหมาย - ResultSize ไม่จำกัด - กรอง {RecipientTypeDetails - eq "UserMailbox" } | ตั้งค่าจดหมาย - AuditEnabled $true
  
[ดูข้อมูลเพิ่มเติม](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

