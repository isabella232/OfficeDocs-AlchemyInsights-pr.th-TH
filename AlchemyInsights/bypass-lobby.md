---
title: เลี่ยงผ่านล็อบบี้
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684969"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="19e2c-102">ควบคุมการตั้งค่าล็อบบี้และระดับการเข้าร่วมในทีม</span><span class="sxs-lookup"><span data-stu-id="19e2c-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="19e2c-103">ถ้าคุณต้องการอนุญาตให้ทุกคนรวมถึงผู้ใช้การโทรเข้าภายนอกและผู้ใช้ที่ไม่ระบุชื่อเพื่อ **เลี่ยงผ่านล็อบบี้**ให้ใช้ PowerShell เพื่อทำงานนี้ให้สำเร็จ</span><span class="sxs-lookup"><span data-stu-id="19e2c-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="19e2c-104">ต่อไปนี้เป็นตัวอย่างของการปรับเปลี่ยนนโยบายการประชุมส่วนกลางสำหรับองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="19e2c-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="19e2c-105">Cmdlet นี้จำเป็นต้องใช้โมดูล PowerShell ของ Skype for Business ในขณะนี้</span><span class="sxs-lookup"><span data-stu-id="19e2c-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="19e2c-106">เมื่อต้องการตั้งค่าให้ใช้ cmdlet นี้ให้ดูที่[นโยบายการจัดการผ่านทาง PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="19e2c-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="19e2c-107">เมื่อคุณตั้งค่านโยบายแล้วคุณจำเป็นต้องนำไปใช้กับผู้ใช้ หรือถ้าคุณได้ปรับเปลี่ยนนโยบายส่วนกลางแล้วโปรแกรมจะนำไปใช้กับผู้ใช้โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="19e2c-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="19e2c-108">สำหรับการเปลี่ยนแปลงนโยบายใดๆคุณจำเป็นต้องรออย่างน้อย **4 ชั่วโมงจนถึง24ชั่วโมง** เพื่อให้นโยบายมีผลบังคับใช้</span><span class="sxs-lookup"><span data-stu-id="19e2c-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="19e2c-109">ตรวจสอบให้แน่ใจว่าได้ตรวจสอบเอกสารด้านล่างก่อนที่จะทำการเปลี่ยนแปลงเหล่านี้เพื่อทำความเข้าใจว่าสิ่งนี้จะช่วยได้อย่างไร</span><span class="sxs-lookup"><span data-stu-id="19e2c-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="19e2c-110">การทำความเข้าใจเกี่ยวกับการควบคุมนโยบายล็อบบี้การประชุมของทีม</span><span class="sxs-lookup"><span data-stu-id="19e2c-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="19e2c-111">การตั้งค่าเหล่านี้จะควบคุมการประชุมที่ผู้เข้าร่วมประชุมรอในล็อบบี้ก่อนที่พวกเขาจะเข้าร่วมการประชุมและระดับของการเข้าร่วมที่พวกเขาได้รับอนุญาตในการประชุม</span><span class="sxs-lookup"><span data-stu-id="19e2c-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="19e2c-112">คุณสามารถใช้ PowerShell เพื่ออัปเดตการตั้งค่านโยบายการประชุมที่ยังไม่ได้นำมาใช้ (ที่มีป้ายชื่อว่า "มาเร็วๆนี้") ในศูนย์การจัดการทีม</span><span class="sxs-lookup"><span data-stu-id="19e2c-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="19e2c-113">ให้ดูที่ด้านล่างสำหรับ cmdlet PowerShell ตัวอย่างที่อนุญาตให้ผู้ใช้ทั้งหมดสามารถเลี่ยงผ่านล็อบบี้ได้</span><span class="sxs-lookup"><span data-stu-id="19e2c-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="19e2c-114">ยอมรับบุคคลที่เป็นนโยบายต่อผู้จัดการ[โดยอัตโนมัติ](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)ที่ควบคุมว่าจะให้ผู้อื่นเข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้จนกว่าพวกเขาจะเข้าร่วมโดยผู้ใช้ที่ได้รับการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="19e2c-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="19e2c-115">[อนุญาตให้ผู้ใช้ที่ไม่ระบุชื่อเริ่มการประชุม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) เป็นนโยบายสำหรับแต่ละตัวจัดระเบียบที่ควบคุมว่าบุคคลที่ไม่ระบุชื่อรวมถึงผู้ใช้ B2B และที่ติดต่อกับภายนอกสามารถเข้าร่วมการประชุมของผู้ใช้โดยไม่มีผู้ใช้ที่ได้รับการรับรองความถูกต้องจากองค์กรในการเข้าร่วม</span><span class="sxs-lookup"><span data-stu-id="19e2c-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="19e2c-116">[อนุญาตให้ผู้ใช้ที่โทรเข้าเพื่อเลี่ยงผ่านล็อบบี้](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)(**เร็วๆนี้**) เป็นนโยบายสำหรับแต่ละตัวจัดระเบียบที่ควบคุมว่าบุคคลที่โทรเข้าเข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้โดยไม่คำนึงถึงการตั้งค่า**บุคคลที่ยอมรับโดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="19e2c-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="19e2c-117">[อนุญาตให้ผู้จัดที่จะแทนที่การตั้งค่าล็อบบี้](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**เร็วๆนี้**) เป็นนโยบายสำหรับแต่ละตัวจัดระเบียบที่ควบคุมว่าผู้จัดการประชุมสามารถแทนที่การตั้งค่าล็อบบี้ที่ตั้งค่าผู้ดูแลได้ **โดยอัตโนมัติ** และ **อนุญาตให้ผู้ใช้โทรเข้าเพื่อเลี่ยงผ่านล็อบบี้** เมื่อพวกเขาจัดกำหนดการการประชุมใหม่</span><span class="sxs-lookup"><span data-stu-id="19e2c-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="19e2c-118">**หมายเหตุ:** อ่าน [จัดการนโยบายการประชุมในทีม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) สำหรับภาพรวมที่สมบูรณ์ของนโยบายการประชุมของ Microsoft team</span><span class="sxs-lookup"><span data-stu-id="19e2c-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
