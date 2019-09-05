---
title: เปิดใช้งานการตรวจสอบจดหมาย
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736272"
---
# <a name="enable-mailbox-auditing"></a>เปิดใช้งานการตรวจสอบจดหมาย

การเปิดใช้งานการตรวจสอบกล่องจดหมายสำหรับผู้ใช้คนเดียวหรือทั้งองค์กรต้องรัน cmdlet ของต่อไปนี้จากเชลล์พลังงานระยะไกล:
  
 **ผู้ใช้คนเดียว**
  
ตั้งค่ากล่องจดหมาย-ตัวตน "Jane Dow"-AuditEnabled $true
  
 **องค์กร**
  
รับกล่องจดหมาย-ResultSize ไม่จำกัด-กรอง {RecipientTypeDetails-eq "UserMailbox"} | การตั้งค่ากล่องจดหมาย-AuditEnabled $true
  
[ศึกษาเพิ่มเติม](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

