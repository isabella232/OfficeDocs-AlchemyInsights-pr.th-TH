---
title: เลื่อนการอัปเกรด Teams ออกไป
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801250"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="bd1c1-102">วิธีการเลื่อนการอัปเกรด Microsoft-Driven Teams</span><span class="sxs-lookup"><span data-stu-id="bd1c1-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="bd1c1-103">**สิ่ง** สําคัญ: เราสามารถช่วยแก้ไขปัญหานี้ให้คุณโดยใช้การวินิจฉัยการสนับสนุน แต่ดูเหมือนว่าคุณไม่ได้ใช้ศูนย์การจัดการใหม่</span><span class="sxs-lookup"><span data-stu-id="bd1c1-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="bd1c1-104">เมื่อต้องการใช้ศูนย์การจัดการใหม่ เลื่อนตัวสลับที่ด้านบนขวาที่ระบุว่า **ศูนย์การจัดการ** ใหม่ ไปทางขวา</span><span class="sxs-lookup"><span data-stu-id="bd1c1-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="bd1c1-105">ใช้ศูนย์การจัดการใหม่ คลิกวิดเจ็ต **ต้องการ** ความช่วยเหลือหรือไม่ พิมพ์ "เลื่อนการอัปเกรด Teams" แล้วตามพร้อมท์เพื่อเรียกใช้การวินิจฉัย</span><span class="sxs-lookup"><span data-stu-id="bd1c1-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="bd1c1-106">หากคุณได้รับการติดต่อสื่อสารเกี่ยวกับการอัปเกรดอัตโนมัติจาก Skype for Business จาก Microsoft for Business ไปยัง Microsoft Teams และคุณต้องการเลื่อนการอัปเกรดอัตโนมัติออกไปในภายหลัง ผู้ดูแลระบบส่วนกลางของคุณสามารถเข้าสู่ระบบพอร์ทัลผู้ดูแลระบบ[ของ Teams](https://admin.teams.microsoft.com/dashboard)และหลังจากเลือกปุ่มรีเฟรชสถานะ ภายใต้การอัปเกรด Microsoft Teamsให้เลือกปุ่ม เลื่อนออกไป</span><span class="sxs-lookup"><span data-stu-id="bd1c1-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="bd1c1-107">เมื่อต้องการดูวันที่ใหม่ในการอัปเกรดอัตโนมัติของผู้เช่าของคุณไปยัง Microsoft Teams ให้รีเฟรชหน้าพอร์ทัลการดูแลระบบ Teams</span><span class="sxs-lookup"><span data-stu-id="bd1c1-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="bd1c1-108">**หมายเหตุ:** **ปุ่ม เลื่อน** ออกไป จะพร้อมใช้งานถ้าคุณได้รับการแจ้งเตือนจากศูนย์ข้อความเกี่ยวกับการอัปเกรดอัตโนมัติเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="bd1c1-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="bd1c1-109">ผู้ดูแลระบบส่วนกลางยังสามารถเรียกใช้ [Get-CsTeamsUpgraderStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) เพื่อเรียนรู้เพิ่มเติมเกี่ยวกับสถานะการอัปเกรดปัจจุบันของพวกเขาได้</span><span class="sxs-lookup"><span data-stu-id="bd1c1-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
