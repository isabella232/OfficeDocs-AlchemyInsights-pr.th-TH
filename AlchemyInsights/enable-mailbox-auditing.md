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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="3d564-102">เปิดใช้งานการตรวจสอบจดหมาย</span><span class="sxs-lookup"><span data-stu-id="3d564-102">Enable mailbox auditing</span></span>

<span data-ttu-id="3d564-103">การเปิดใช้งานการตรวจสอบกล่องจดหมายสำหรับผู้ใช้คนเดียวหรือทั้งองค์กรต้องรัน cmdlet ของต่อไปนี้จากเชลล์พลังงานระยะไกล:</span><span class="sxs-lookup"><span data-stu-id="3d564-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="3d564-104">**ผู้ใช้คนเดียว**</span><span class="sxs-lookup"><span data-stu-id="3d564-104">**Single User**</span></span>
  
<span data-ttu-id="3d564-105">ตั้งค่ากล่องจดหมาย-ตัวตน "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="3d564-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="3d564-106">**องค์กร**</span><span class="sxs-lookup"><span data-stu-id="3d564-106">**Organization**</span></span>
  
<span data-ttu-id="3d564-107">รับกล่องจดหมาย-ResultSize ไม่จำกัด-กรอง {RecipientTypeDetails-eq "UserMailbox"} | การตั้งค่ากล่องจดหมาย-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="3d564-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="3d564-108">ศึกษาเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="3d564-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

