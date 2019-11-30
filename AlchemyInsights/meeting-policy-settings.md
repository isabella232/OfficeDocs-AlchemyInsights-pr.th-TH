---
title: การตั้งค่านโยบายการประชุม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627593"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="55de4-102">จัดการนโยบายการประชุมใน Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="55de4-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="55de4-103">นโยบายการประชุมจะใช้ในการควบคุมคุณลักษณะที่พร้อมใช้งานสำหรับผู้เข้าร่วมประชุมสำหรับการประชุมที่มีการจัดตารางการผลิตระดับผู้ใช้ในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="55de4-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="55de4-104">คุณลักษณะบางอย่างของนโยบายการประชุมอาจไม่ได้ดำเนินการในศูนย์กลางการดูแลระบบ (ซึ่งมีป้ายชื่อ "เร็วๆนี้" ในเอกสารประกอบ)</span><span class="sxs-lookup"><span data-stu-id="55de4-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="55de4-105">ในกรณีนี้หรือถ้าคุณได้รับข้อผิดพลาดเช่น "เราไม่สามารถปรับปรุงนโยบายในขณะนี้แต่ลองอีกครั้งในภายหลัง" ในศูนย์กลางการดูแล Microsoft Teams เราขอแนะนำให้คุณใช้ PowerShell เพื่อสร้างหรือปรับเปลี่ยนนโยบายการประชุมของทีม</span><span class="sxs-lookup"><span data-stu-id="55de4-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="55de4-106">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการประชุมโปรดดูทรัพยากรต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="55de4-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="55de4-107">หากต้องการเรียนรู้เกี่ยวกับการสร้างนโยบายทำการเปลี่ยนแปลงและกำหนดผู้ใช้ให้กับนโยบายโปรดดูที่[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="55de4-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="55de4-108">เพื่อทำการเปลี่ยนแปลงนโยบายโดยใช้ cmdlet[ของ powershell ดูภาพรวมของทีม powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="55de4-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="55de4-109">คุณจำเป็นต้องใช้[Skype สำหรับโมดูล PowerShell ธุรกิจ](https://www.microsoft.com/download/details.aspx?id=39366)สำหรับนโยบายการประชุมทีม</span><span class="sxs-lookup"><span data-stu-id="55de4-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="55de4-110">ตรวจทาน[เอกสารการ cmdlet ของ \*-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="55de4-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="55de4-111">**หมายเหตุ:** การเปลี่ยนแปลงนโยบายอาจใช้เวลาถึง24ชั่วโมงจึงจะมีผลสำหรับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="55de4-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="55de4-112">คุณอาจไม่สามารถทำการเปลี่ยนแปลงนโยบายที่สร้างขึ้นใหม่ได้ทันที รอ4ชั่วโมงและพยายามที่จะปรับเปลี่ยนนโยบายที่สร้างขึ้นใหม่อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="55de4-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="55de4-113">หากคุณยังคงมีปัญหาอยู่ให้ลองใช้ PowerShell</span><span class="sxs-lookup"><span data-stu-id="55de4-113">If you're still having problems, try PowerShell.</span></span>  