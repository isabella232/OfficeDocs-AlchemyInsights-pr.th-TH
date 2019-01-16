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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="caeab-102">เปิดใช้งานการตรวจสอบของกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="caeab-102">Enable mailbox auditing</span></span>

<span data-ttu-id="caeab-103">เมื่อต้องการเปิดใช้งานการตรวจสอบของกล่องจดหมายสำหรับผู้ใช้คนเดียวหรือทั้งองค์กร ต้องรันการ cmdlet ของต่อไปนี้จากเชลล์พลังงานระยะไกล:</span><span class="sxs-lookup"><span data-stu-id="caeab-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="caeab-104">**ผู้ใช้คนเดียว**</span><span class="sxs-lookup"><span data-stu-id="caeab-104">**Single User**</span></span>
  
<span data-ttu-id="caeab-105">ตั้งค่าจดหมาย - รหัสประจำตัว "เจนด" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="caeab-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="caeab-106">**องค์กร**</span><span class="sxs-lookup"><span data-stu-id="caeab-106">**Organization**</span></span>
  
<span data-ttu-id="caeab-107">รับจดหมาย - ResultSize ไม่จำกัด - กรอง {RecipientTypeDetails - eq "UserMailbox" } | ตั้งค่าจดหมาย - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="caeab-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="caeab-108">ดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="caeab-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

