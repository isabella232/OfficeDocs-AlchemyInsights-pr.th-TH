---
title: เปิดใช้งานการตรวจสอบของกล่องจดหมาย
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 3a7ffccadf6b415f7dd0d0871d368402332a0cd7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916759"
---
# <a name="enable-mailbox-auditing"></a>เปิดใช้งานการตรวจสอบของกล่องจดหมาย

เมื่อต้องการเปิดใช้งานการตรวจสอบของกล่องจดหมายสำหรับผู้ใช้คนเดียวหรือทั้งองค์กร ต้องรันการ cmdlet ของต่อไปนี้จากเชลล์พลังงานระยะไกล:
  
 **ผู้ใช้คนเดียว**
  
ตั้งค่าจดหมาย - รหัสประจำตัว "เจนด" - AuditEnabled $true
  
 **องค์กร**
  
รับจดหมาย - ResultSize ไม่จำกัด - กรอง {RecipientTypeDetails - eq "UserMailbox" } | ตั้งค่าจดหมาย - AuditEnabled $true
  
[ดูข้อมูลเพิ่มเติม](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

