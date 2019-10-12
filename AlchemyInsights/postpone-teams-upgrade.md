---
title: 'เลื่อนทีมอัพเกรด '
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: bee729ffe9fbbf379612c658cdad25b1fbfdd0ab
ms.sourcegitcommit: add3ed8156af0a0a8b2659e906dfd60144346124
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/11/2019
ms.locfileid: "37469349"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="f06d8-102">วิธีการเลื่อนการปรับรุ่นทีมที่ขับเคลื่อนด้วย Microsoft</span><span class="sxs-lookup"><span data-stu-id="f06d8-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="f06d8-103">ถ้าคุณได้รับการสื่อสารเกี่ยวกับการปรับรุ่นอัตโนมัติที่ขับเคลื่อนด้วย Microsoft จาก Skype สำหรับธุรกิจไปยัง Microsoft Teams และคุณต้องการเลื่อนการปรับรุ่นอัตโนมัติเป็นวันที่หลังจากนั้น Office ๓๖๕ผู้ดูแลส่วนกลางของคุณสามารถล็อกอินเข้าสู่[พอร์ทัล Admin ทีม](https://admin.teams.microsoft.com/dashboard)และเลือก ปุ่ม**เลื่อน**</span><span class="sxs-lookup"><span data-stu-id="f06d8-103">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Office 365 Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and select the **Postpone** button.</span></span> <span data-ttu-id="f06d8-104">หากต้องการดูวันที่ใหม่สำหรับการอัพเกรดอัตโนมัติของผู้เช่าของคุณให้กับ Microsoft Teams ให้รีเฟรชหน้าพอร์ทัล Admin ทีม</span><span class="sxs-lookup"><span data-stu-id="f06d8-104">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="f06d8-105">**หมายเหตุ:** ปุ่ม**เลื่อน**จะพร้อมใช้งานเฉพาะเมื่อคุณได้รับการแจ้งเตือนศูนย์ข้อความเกี่ยวกับการอัพเกรดอัตโนมัติเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="f06d8-105">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="f06d8-106">Office ๓๖๕ผู้ดูแลส่วนกลางสามารถเรียกใช้[รับ-CsTeamsUpgradeStatus](https://docs.microsoft.com/en-us/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps)เพื่อเรียนรู้เพิ่มเติมเกี่ยวกับสถานะการปรับรุ่นปัจจุบันของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="f06d8-106">Office 365 Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/en-us/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span> 