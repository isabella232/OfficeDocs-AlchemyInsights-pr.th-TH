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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376873"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="9f744-102">ควบคุมการตั้งค่าและระดับการเข้าร่วมของล็อบบี้</span><span class="sxs-lookup"><span data-stu-id="9f744-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="9f744-103">การตั้งค่าเหล่านี้จะควบคุมผู้เข้าร่วมประชุมที่รออยู่ในล็อบบี้ก่อนที่จะเข้ารับการประชุมและระดับการเข้าร่วมประชุมที่ได้รับอนุญาต</span><span class="sxs-lookup"><span data-stu-id="9f744-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="9f744-104">คุณสามารถใช้ Powershell เพื่อปรับปรุงการตั้งค่านโยบายการประชุมที่ยังไม่ได้ดำเนินการ (ที่มีป้ายชื่อ "เร็วๆนี้") ในศูนย์การจัดการทีม</span><span class="sxs-lookup"><span data-stu-id="9f744-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="9f744-105">ดูด้านล่างสำหรับตัวอย่าง cmdlet PowerShell ที่ช่วยให้ผู้ใช้ทั้งหมดที่จะข้ามล็อบบี้</span><span class="sxs-lookup"><span data-stu-id="9f744-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="9f744-106">[ยอมรับผู้ใช้โดยอัตโนมัติ](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)เป็นนโยบายต่อการจัดการที่ควบคุมว่าผู้คนเข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้จนกว่าพวกเขาจะได้รับการตรวจสอบโดยผู้ที่รับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="9f744-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="9f744-107">[อนุญาตให้บุคคลที่ไม่ระบุชื่อเริ่มการประชุม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)เป็นนโยบายต่อตัวจัดการที่ควบคุมว่าบุคคลที่ไม่ระบุชื่อรวมถึงผู้ใช้แบบ B2B และที่ติดต่อกับภายนอกสามารถเข้าร่วมการประชุมของผู้ใช้ได้โดยไม่มีผู้ใช้ที่รับรองความถูกต้องจากองค์กรในการเข้างาน</span><span class="sxs-lookup"><span data-stu-id="9f744-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="9f744-108">[อนุญาตให้ผู้ใช้โทรออกในการข้ามล็อบบี้](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)(**เร็วๆนี้**) เป็นนโยบายต่อการจัดการที่ควบคุมว่าผู้ที่เรียกเลขหมายโดยโทรศัพท์เข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้โดยไม่คำนึงถึงการตั้งค่า**ผู้คนที่ยอมรับโดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="9f744-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="9f744-109">[อนุญาตให้ผู้จัดการแทนที่การตั้งค่าล็อบบี้](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)(**เร็วๆนี้**) เป็นนโยบายต่อตัวจัดการที่ควบคุมว่าผู้จัดการประชุมสามารถแทนที่การตั้งค่าล็อบบี้ที่ผู้ดูแลตั้งค่า**โดยอัตโนมัติยอมรับคน**และ**อนุญาตให้มีการเรียกเลขหมาย ผู้ใช้ที่จะข้ามล็อบบี้**เมื่อพวกเขาจัดกำหนดการการประชุมใหม่</span><span class="sxs-lookup"><span data-stu-id="9f744-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="9f744-110">**หมายเหตุ:** อ่าน[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)เพื่อดูภาพรวมทั้งหมดของนโยบายการประชุมของ Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9f744-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="9f744-111">**ตัวอย่างของ PowerShell**</span><span class="sxs-lookup"><span data-stu-id="9f744-111">**PowerShell example**</span></span>

<span data-ttu-id="9f744-112">หากคุณต้องการอนุญาตให้ทุกคนรวมถึงผู้ใช้ภายนอกหรือไม่ระบุชื่อให้ข้ามล็อบบี้คุณยังสามารถใช้ PowerShell เพื่อทำงานนี้ให้สำเร็จได้</span><span class="sxs-lookup"><span data-stu-id="9f744-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="9f744-113">ต่อไปนี้เป็นตัวอย่างของการปรับเปลี่ยนนโยบายการประชุมส่วนกลางสำหรับองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="9f744-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="9f744-114">(โปรดตรวจสอบเอกสารดังกล่าวข้างต้นก่อนทำการเปลี่ยนแปลงเหล่านี้เพื่อให้เข้าใจว่าสิ่งนี้ช่วยได้อย่างไร)</span><span class="sxs-lookup"><span data-stu-id="9f744-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="9f744-115">ชุด-CsTeamsMeetingPolicy-อัตลักษณ์ทั่วโลก-AutoAdmittedUsers "ทุกคน"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="9f744-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="9f744-116">สำหรับข้อมูลเพิ่มเติมโปรดดูที่[ชุด-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="9f744-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
