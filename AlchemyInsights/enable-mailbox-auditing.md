---
title: เปิดใช้งานการตรวจสอบกล่องจดหมาย
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703590"
---
# <a name="enable-mailbox-auditing"></a>เปิดใช้งานการตรวจสอบกล่องจดหมาย

เมื่อต้องการเปิดใช้งานการตรวจสอบกล่องจดหมายสําหรับผู้ใช้คนเดียวหรือทั้งองค์กร cmdlet ต่อไปนี้ต้องเรียกใช้จากเชลล์พลังงานระยะไกล:
  
 **ผู้ใช้คนเดียว**
  
ตั้งค่ากล่องจดหมาย -ข้อมูลเฉพาะตัว "Jane Dow" -auditenabled $true
  
 **องค์กร**
  
รับกล่องจดหมาย -Resultขนาดไม่จํากัด -Filter {RecipientTypeรายละเอียด -eq "UserMailbox"} | ตั้งค่ากล่องจดหมาย - $true AuditEnabled
  
[ศึกษาเพิ่มเติม](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

