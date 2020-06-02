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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="14a71-102">เปิดใช้งานการตรวจสอบกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="14a71-102">Enable mailbox auditing</span></span>

<span data-ttu-id="14a71-103">เมื่อต้องการเปิดใช้งานการตรวจสอบกล่องจดหมายสําหรับผู้ใช้คนเดียวหรือองค์กรทั้งหมด cmdlets ต่อไปนี้ต้องเรียกใช้จากเชลล์พลังงานระยะไกล:</span><span class="sxs-lookup"><span data-stu-id="14a71-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="14a71-104">**ผู้ใช้รายเดียว**</span><span class="sxs-lookup"><span data-stu-id="14a71-104">**Single User**</span></span>
  
<span data-ttu-id="14a71-105">กล่องจดหมายการตั้งค่า -identity "Jane Dow" -auditenabled $true</span><span class="sxs-lookup"><span data-stu-id="14a71-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="14a71-106">**องค์กร**</span><span class="sxs-lookup"><span data-stu-id="14a71-106">**Organization**</span></span>
  
<span data-ttu-id="14a71-107">รับกล่องจดหมาย -ผลลัพธ์ขนาดไม่ จํากัด -กรองผู้รับชนิดDetails -eq "UserMailbox"} | $trueกล่องจดหมายเซ็ต -AuditEnabled</span><span class="sxs-lookup"><span data-stu-id="14a71-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="14a71-108">ศึกษาเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="14a71-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

