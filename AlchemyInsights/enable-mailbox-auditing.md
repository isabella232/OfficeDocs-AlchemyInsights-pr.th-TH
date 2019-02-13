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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="811d7-102">เปิดใช้งานการตรวจสอบของกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="811d7-102">Enable mailbox auditing</span></span>

<span data-ttu-id="811d7-103">เมื่อต้องการเปิดใช้งานการตรวจสอบของกล่องจดหมายสำหรับผู้ใช้คนเดียวหรือทั้งองค์กร ต้องรันการ cmdlet ของต่อไปนี้จากเชลล์พลังงานระยะไกล:</span><span class="sxs-lookup"><span data-stu-id="811d7-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="811d7-104">**ผู้ใช้คนเดียว**</span><span class="sxs-lookup"><span data-stu-id="811d7-104">**Single User**</span></span>
  
<span data-ttu-id="811d7-105">ตั้งค่าจดหมาย - รหัสประจำตัว "เจนด" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="811d7-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="811d7-106">**องค์กร**</span><span class="sxs-lookup"><span data-stu-id="811d7-106">**Organization**</span></span>
  
<span data-ttu-id="811d7-107">รับจดหมาย - ResultSize ไม่จำกัด - กรอง {RecipientTypeDetails - eq "UserMailbox" } | ตั้งค่าจดหมาย - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="811d7-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="811d7-108">ดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="811d7-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

