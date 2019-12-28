---
title: ล็อบบี้
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889101"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="7ffe2-102">ควบคุมการตั้งค่าล็อบบี้และระดับการเข้าร่วมทีม</span><span class="sxs-lookup"><span data-stu-id="7ffe2-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="7ffe2-103">หากคุณต้องการอนุญาตให้ทุกคนรวมถึงการเรียกเลขหมายภายนอกและผู้ใช้ที่ไม่ระบุชื่อให้**ข้ามล็อบบี้**ให้ใช้ PowerShell เพื่อทำงานนี้ให้สำเร็จ</span><span class="sxs-lookup"><span data-stu-id="7ffe2-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="7ffe2-104">ต่อไปนี้เป็นตัวอย่างของการปรับเปลี่ยนนโยบายการประชุมส่วนกลางสำหรับองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="7ffe2-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="7ffe2-105">Cmdlet นี้จำเป็นต้องใช้ Skype สำหรับโมดูล PowerShell ธุรกิจในขณะนี้</span><span class="sxs-lookup"><span data-stu-id="7ffe2-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="7ffe2-106">หากต้องการรับการตั้งค่าเพื่อใช้ cmdlet นี้ให้ตรวจสอบ[นโยบายการจัดการผ่านทาง PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="7ffe2-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="7ffe2-107">เมื่อคุณตั้งค่านโยบายแล้วคุณจะต้องนำไปใช้กับผู้ใช้ หรือถ้าคุณปรับเปลี่ยนนโยบายสากลระบบจะนำไปใช้กับผู้ใช้โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="7ffe2-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="7ffe2-108">สำหรับการเปลี่ยนแปลงนโยบายใดๆคุณต้องรออย่างน้อย**4 ชั่วโมงจนถึง24ชั่วโมง**เพื่อให้นโยบายมีผลบังคับใช้</span><span class="sxs-lookup"><span data-stu-id="7ffe2-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="7ffe2-109">ตรวจสอบให้แน่ใจว่าได้ตรวจสอบเอกสารด้านล่างก่อนที่จะทำการเปลี่ยนแปลงเหล่านี้เพื่อให้เข้าใจว่าสิ่งนี้ช่วยได้อย่างไร</span><span class="sxs-lookup"><span data-stu-id="7ffe2-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="7ffe2-110">ทำความเข้าใจเกี่ยวกับการควบคุมทีมงานการประชุมนโยบายล็อบบี้</span><span class="sxs-lookup"><span data-stu-id="7ffe2-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="7ffe2-111">การตั้งค่าเหล่านี้จะควบคุมผู้เข้าร่วมประชุมที่รออยู่ในล็อบบี้ก่อนที่จะเข้ารับการประชุมและระดับการเข้าร่วมประชุมที่ได้รับอนุญาต</span><span class="sxs-lookup"><span data-stu-id="7ffe2-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="7ffe2-112">คุณสามารถใช้ PowerShell เพื่อปรับปรุงการตั้งค่านโยบายการประชุมที่ยังไม่ได้ดำเนินการ (ที่มีป้ายชื่อ "เร็วๆนี้") ในศูนย์การจัดการทีม</span><span class="sxs-lookup"><span data-stu-id="7ffe2-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="7ffe2-113">ดูด้านล่างสำหรับตัวอย่าง cmdlet PowerShell ที่ช่วยให้ผู้ใช้ทั้งหมดที่จะข้ามล็อบบี้</span><span class="sxs-lookup"><span data-stu-id="7ffe2-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="7ffe2-114">[ยอมรับผู้ใช้โดยอัตโนมัติ](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)เป็นนโยบายต่อการจัดการที่ควบคุมว่าผู้คนเข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้จนกว่าพวกเขาจะได้รับการตรวจสอบโดยผู้ที่รับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="7ffe2-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="7ffe2-115">[อนุญาตให้บุคคลที่ไม่ระบุชื่อเริ่มการประชุม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)เป็นนโยบายต่อตัวจัดการที่ควบคุมว่าบุคคลที่ไม่ระบุชื่อรวมถึงผู้ใช้แบบ B2B และที่ติดต่อกับภายนอกสามารถเข้าร่วมการประชุมของผู้ใช้ได้โดยไม่มีผู้ใช้ที่รับรองความถูกต้องจากองค์กรในการเข้างาน</span><span class="sxs-lookup"><span data-stu-id="7ffe2-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="7ffe2-116">[อนุญาตให้ผู้ใช้โทรออกในการข้ามล็อบบี้](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)(**เร็วๆนี้**) เป็นนโยบายต่อการจัดการที่ควบคุมว่าผู้ที่เรียกเลขหมายโดยโทรศัพท์เข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้โดยไม่คำนึงถึงการตั้งค่า**ผู้คนที่ยอมรับโดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="7ffe2-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="7ffe2-117">[อนุญาตให้ผู้จัดทำการแทนที่การตั้งค่าล็อบบี้](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)(**เร็วๆนี้**) เป็นนโยบายสำหรับแต่ละตัวจัดการที่ควบคุมว่าการประชุมผู้จัดการสามารถแทนที่การตั้งค่าล็อบบี้ที่ผู้ดูแลระบบตั้งค่าไว้**โดยอัตโนมัติยอมรับบุคคล**และ**อนุญาตให้ใช้การเรียกเลขหมายในการข้ามล็อบบี้**เมื่อพวกเขาจัดตารางเวลาการประชุมใหม่</span><span class="sxs-lookup"><span data-stu-id="7ffe2-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="7ffe2-118">**หมายเหตุ:** อ่าน[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)เพื่อดูภาพรวมทั้งหมดของนโยบายการประชุมของ Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7ffe2-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
