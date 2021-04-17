---
title: การเลี่ยงผ่านล็อบบี้
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820053"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="ec9d1-102">ควบคุมการตั้งค่าล็อบบี้และระดับการมีส่วนร่วมใน Teams</span><span class="sxs-lookup"><span data-stu-id="ec9d1-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="ec9d1-103">ถ้าคุณต้องการอนุญาตให้ทุกคน รวมถึง Dial-in, ผู้ใช้ภายนอก และผู้ใช้ที่ไม่ระบุชื่อ สามารถเลี่ยงผ่านล็อบบี้ ได้ ให้ใช้ PowerShell เพื่อทํางานนี้ให้เสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="ec9d1-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="ec9d1-104">ต่อไปนี้เป็นตัวอย่างของการปรับเปลี่ยนนโยบายการประชุมส่วนกลางขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="ec9d1-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="ec9d1-105">cmdlet นี้ต้องใช้มอดูล PowerShell ของ Skype for Business ในขณะนี้</span><span class="sxs-lookup"><span data-stu-id="ec9d1-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="ec9d1-106">เมื่อต้องการตั้งค่าเพื่อใช้ cmdlet นี้ ให้ตรวจสอบ[การจัดการนโยบายผ่านทาง PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="ec9d1-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="ec9d1-107">เมื่อคุณตั้งค่านโยบายแล้ว คุณจึงต้องปรับใช้นโยบายกับผู้ใช้ หรือหากคุณปรับเปลี่ยนนโยบายส่วนกลาง นโยบายจะมีผลบังคับใช้กับผู้ใช้โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="ec9d1-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="ec9d1-108">เพื่อให้การเปลี่ยนแปลงนโยบายมีผล อย่างน้อย **4 ชั่วโมงจึงจะถึง 24** ชั่วโมงเพื่อให้นโยบายมีผล</span><span class="sxs-lookup"><span data-stu-id="ec9d1-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="ec9d1-109">อย่าลืมตรวจทานเอกสารประกอบด้านล่างก่อนการเปลี่ยนแปลงเหล่านี้เพื่อเข้าใจว่าสิ่งนี้อนุญาตคืออะไร</span><span class="sxs-lookup"><span data-stu-id="ec9d1-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="ec9d1-110">การเข้าใจตัวควบคุมนโยบายล็อบบี้การประชุม Teams</span><span class="sxs-lookup"><span data-stu-id="ec9d1-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="ec9d1-111">การตั้งค่าเหล่านี้จะควบคุมว่าผู้เข้าร่วมการประชุมคนใดจะต้องรอในล็อบบี้ก่อนได้รับการยอมรับให้เข้าร่วมการประชุมและระดับการมีส่วนร่วมในการประชุม</span><span class="sxs-lookup"><span data-stu-id="ec9d1-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="ec9d1-112">คุณสามารถใช้ PowerShell เพื่ออัปเดตการตั้งค่านโยบายการประชุมที่ยังไม่ได้ปรับใช้ (ที่มีป้ายชื่อ "เร็วๆ นี้") ในศูนย์การจัดการ Teams</span><span class="sxs-lookup"><span data-stu-id="ec9d1-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="ec9d1-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span><span class="sxs-lookup"><span data-stu-id="ec9d1-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="ec9d1-114">[ยอมรับบุคคลโดยอัตโนมัติ](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) เป็นนโยบายต่อผู้จัดที่จะควบคุมว่าบุคคลที่เข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้จนกว่าได้รับการยอมรับจากผู้ใช้ที่ได้รับการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="ec9d1-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="ec9d1-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federrated users, can join the user's meeting without an authenticated user from the organization in attendance.</span><span class="sxs-lookup"><span data-stu-id="ec9d1-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="ec9d1-116">[อนุญาตให้ผู้ใช้โทร](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)เข้าเพื่อข้ามล็อบบี้ **(เร็ว** ๆ นี้ ) เป็นนโยบายต่อผู้จัดการประชุมที่ควบคุมว่าบุคคลที่โทรเข้าทางโทรศัพท์เข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้โดยไม่เกี่ยวกับการตั้งค่า ยอมรับ **บุคคลโดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="ec9d1-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="ec9d1-117">[อนุญาตให้](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)ผู้จัดการประชุมแทนที่การตั้งค่าล็อบบี้ **(เร็ว** ๆ นี้ ) เป็นนโยบายต่อผู้จัดการประชุมที่ควบคุมว่าผู้จัดการประชุมสามารถแทนที่การตั้งค่าล็อบบี้ที่ผู้ดูแลระบบตั้งค่าในยอมรับบุคคลและอนุญาตให้ผู้ใช้โทรเข้าโดยอัตโนมัติ หรือไม่เพื่อเลี่ยงผ่านล็อบบี้เมื่อพวกเขาจัดเวลาการประชุมใหม่</span><span class="sxs-lookup"><span data-stu-id="ec9d1-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="ec9d1-118">**หมายเหตุ:** อ่าน [จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) เพื่อดูภาพรวมโดยสมบูรณ์ของนโยบายการประชุม Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ec9d1-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
