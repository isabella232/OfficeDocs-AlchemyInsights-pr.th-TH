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
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506973"
---
# <a name="enable-mailbox-auditing"></a>เปิดใช้งานการตรวจสอบกล่องจดหมาย

เมื่อต้องการเปิดใช้งานการตรวจสอบกล่องจดหมายสําหรับผู้ใช้คนเดียวหรือองค์กรทั้งหมด cmdlets ต่อไปนี้ต้องเรียกใช้จากเชลล์พลังงานระยะไกล:
  
 **ผู้ใช้รายเดียว**
  
กล่องจดหมายการตั้งค่า -identity "Jane Dow" -auditenabled $true
  
 **องค์กร**
  
รับกล่องจดหมาย -ผลลัพธ์ขนาดไม่ จํากัด -กรองผู้รับชนิดDetails -eq "UserMailbox"} | $trueกล่องจดหมายเซ็ต -AuditEnabled
  
[ศึกษาเพิ่มเติม](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

