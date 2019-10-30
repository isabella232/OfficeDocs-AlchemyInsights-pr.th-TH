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
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768459"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="e7fb3-102">ควบคุมการตั้งค่าและระดับการเข้าร่วมของล็อบบี้</span><span class="sxs-lookup"><span data-stu-id="e7fb3-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="e7fb3-103">หากคุณต้องการอนุญาตให้ทุกคนรวมถึงการเรียกเลขหมายภายนอกและผู้ใช้ที่ไม่ระบุชื่อเพื่อข้ามล็อบบี้ใน Microsoft Teams คุณสามารถใช้ PowerShell เพื่อทำได้</span><span class="sxs-lookup"><span data-stu-id="e7fb3-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="e7fb3-104">นี่คือตัวอย่างของการปรับเปลี่ยนนโยบายการประชุมทั่วโลกสำหรับองค์กรของคุณ:</span><span class="sxs-lookup"><span data-stu-id="e7fb3-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="e7fb3-105">Cmdlet นี้จำเป็นต้องใช้ Skype สำหรับโมดูล PowerShell ธุรกิจในขณะนี้</span><span class="sxs-lookup"><span data-stu-id="e7fb3-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="e7fb3-106">หากต้องการรับการตั้งค่าเพื่อใช้ cmdlet นี้ให้ตรวจสอบ[นโยบายการจัดการผ่านทาง PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="e7fb3-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="e7fb3-107">คุณสามารถตั้งค่านโยบายใหม่ซึ่งคุณจะต้องนำไปใช้กับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="e7fb3-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="e7fb3-108">ถ้าคุณปรับเปลี่ยนนโยบายส่วนกลางจะใช้กับผู้ใช้โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="e7fb3-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="e7fb3-109">สำหรับการเปลี่ยนแปลงนโยบายใดๆที่คุณต้องรออย่างน้อย4ชั่วโมงและสูงสุด24ชั่วโมงเพื่อให้นโยบายมีผลบังคับใช้</span><span class="sxs-lookup"><span data-stu-id="e7fb3-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="e7fb3-110">ตรวจสอบให้แน่ใจว่าได้ตรวจสอบเอกสารด้านล่างก่อนที่จะทำการเปลี่ยนแปลงเหล่านี้เพื่อให้เข้าใจว่าสิ่งนี้ช่วยได้อย่างไร</span><span class="sxs-lookup"><span data-stu-id="e7fb3-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="e7fb3-111">ทำความเข้าใจเกี่ยวกับการควบคุมทีมงานการประชุมนโยบายล็อบบี้</span><span class="sxs-lookup"><span data-stu-id="e7fb3-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="e7fb3-112">[ยอมรับผู้ใช้โดยอัตโนมัติ](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)เป็นนโยบายต่อการจัดการที่ควบคุมว่าผู้คนเข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้จนกว่าพวกเขาจะได้รับการตรวจสอบโดยผู้ที่รับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="e7fb3-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="e7fb3-113">[อนุญาตให้บุคคลที่ไม่ระบุชื่อเริ่มการประชุม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)เป็นนโยบายต่อตัวจัดการที่ควบคุมว่าบุคคลที่ไม่ระบุชื่อรวมถึงผู้ใช้แบบ B2B และที่ติดต่อกับภายนอกสามารถเข้าร่วมการประชุมของผู้ใช้ได้โดยไม่มีผู้ใช้ที่รับรองความถูกต้องจากองค์กรในการเข้างาน</span><span class="sxs-lookup"><span data-stu-id="e7fb3-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="e7fb3-114">[อนุญาตให้ผู้ใช้โทรออกในการข้ามล็อบบี้](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)(**เร็วๆนี้**) เป็นนโยบายต่อการจัดการที่ควบคุมว่าผู้ที่เรียกเลขหมายโดยโทรศัพท์เข้าร่วมการประชุมโดยตรงหรือรอในล็อบบี้โดยไม่คำนึงถึงการตั้งค่า**ผู้คนที่ยอมรับโดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="e7fb3-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="e7fb3-115">[อนุญาตให้ผู้จัดการแทนที่การตั้งค่าล็อบบี้](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)(**เร็วๆนี้**) เป็นนโยบายต่อตัวจัดการที่ควบคุมว่าผู้จัดการประชุมสามารถแทนที่การตั้งค่าล็อบบี้ที่ผู้ดูแลตั้งค่า**โดยอัตโนมัติยอมรับคน**และ**อนุญาตให้มีการเรียกเลขหมาย ผู้ใช้ที่จะข้ามล็อบบี้**เมื่อพวกเขาจัดกำหนดการการประชุมใหม่</span><span class="sxs-lookup"><span data-stu-id="e7fb3-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="e7fb3-116">**หมายเหตุ:** อ่าน[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)เพื่อดูภาพรวมทั้งหมดของนโยบายการประชุมของ Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e7fb3-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
