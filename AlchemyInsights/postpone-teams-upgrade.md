---
title: เลื่อนการอัปเกรดทีม
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
ms.openlocfilehash: fcf724e335bd6a7cb4801d9b2789447befc06ff7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912530"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="7548f-102">วิธีการเลื่อนการอัปเกรดทีมที่ขับเคลื่อนด้วย Microsoft</span><span class="sxs-lookup"><span data-stu-id="7548f-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="7548f-103">**สิ่งสำคัญ**: เราสามารถช่วยแก้ไขปัญหานี้ให้คุณได้โดยใช้การวินิจฉัยการสนับสนุนแต่ดูเหมือนว่าคุณไม่ได้ใช้ศูนย์การจัดการใหม่</span><span class="sxs-lookup"><span data-stu-id="7548f-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="7548f-104">เมื่อต้องการใช้ศูนย์การจัดการใหม่ให้เลื่อนตัวสลับที่ด้านบนขวาที่ระบุว่า **ศูนย์การจัดการใหม่** ทางด้านขวา</span><span class="sxs-lookup"><span data-stu-id="7548f-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="7548f-105">การใช้ศูนย์การจัดการใหม่ให้คลิก **ต้องการความช่วยเหลือ** วิดเจ็ตพิมพ์ "เลื่อนทีมอัปเกรด" แล้วทำตามพร้อมท์เพื่อเรียกใช้การวิเคราะห์การเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="7548f-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="7548f-106">ถ้าคุณได้รับการติดต่อสื่อสารเกี่ยวกับการอัปเกรดอัตโนมัติจาก Skype for Business ไปยังทีม Microsoft และคุณต้องการเลื่อนการอัปเกรดอัตโนมัติเป็นวันที่ภายหลังผู้ดูแลระบบส่วนกลางของคุณสามารถลงชื่อเข้าใช้[พอร์ทัลการจัดการทีม](https://admin.teams.microsoft.com/dashboard)และหลังจากเลือกปุ่ม**สถานะการรีเฟรช**ภายใต้การอัปเกรดทีม Microsoft ให้เลือกปุ่ม**เลื่อน**</span><span class="sxs-lookup"><span data-stu-id="7548f-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="7548f-107">เมื่อต้องการดูวันที่ใหม่สำหรับการอัปเกรดอัตโนมัติของผู้เช่าของคุณไปยังทีม Microsoft ให้รีเฟรชหน้าพอร์ทัลการจัดการทีม</span><span class="sxs-lookup"><span data-stu-id="7548f-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="7548f-108">**หมายเหตุ:** ปุ่ม **เลื่อน** จะพร้อมใช้งานก็ต่อเมื่อคุณได้รับการแจ้งเตือนของศูนย์ข้อความเกี่ยวกับการอัปเกรดโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="7548f-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="7548f-109">ผู้ดูแลระบบส่วนกลางยังสามารถเรียกใช้ [CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) เพื่อเรียนรู้เพิ่มเติมเกี่ยวกับสถานะการอัปเกรดปัจจุบันของพวกเขาได้</span><span class="sxs-lookup"><span data-stu-id="7548f-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
