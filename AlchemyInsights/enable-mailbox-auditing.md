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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="f1bb1-102">เปิดใช้งานการตรวจสอบกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="f1bb1-102">Enable mailbox auditing</span></span>

<span data-ttu-id="f1bb1-103">เมื่อต้องการเปิดใช้งานการตรวจสอบกล่องจดหมายสำหรับผู้ใช้คนเดียวหรือทั้งองค์กรจะต้องเรียกใช้ cmdlet ต่อไปนี้จาก Shell Power ระยะไกล:</span><span class="sxs-lookup"><span data-stu-id="f1bb1-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="f1bb1-104">**ผู้ใช้คนเดียว**</span><span class="sxs-lookup"><span data-stu-id="f1bb1-104">**Single User**</span></span>
  
<span data-ttu-id="f1bb1-105">ตั้งค่ากล่องจดหมาย-ข้อมูลประจำตัว "Jane AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="f1bb1-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="f1bb1-106">**องค์กร**</span><span class="sxs-lookup"><span data-stu-id="f1bb1-106">**Organization**</span></span>
  
<span data-ttu-id="f1bb1-107">กล่องจดหมาย-ResultSize ไม่จำกัด-ตัวกรอง {RecipientTypeDetails-eq "UserMailbox"} | ตั้งค่ากล่องจดหมาย-$true AuditEnabled</span><span class="sxs-lookup"><span data-stu-id="f1bb1-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="f1bb1-108">ศึกษาเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="f1bb1-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

