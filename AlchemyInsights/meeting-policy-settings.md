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
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042863"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="7d523-102">จัดการนโยบายการประชุมในทีมของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="7d523-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="7d523-103">**หมายเหตุ: อาจใช้เวลาถึง24ชั่วโมงสำหรับการเปลี่ยนแปลงนโยบายที่จะมีผลสำหรับผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="7d523-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="7d523-104">คุณอาจไม่สามารถทำการเปลี่ยนแปลงนโยบายที่สร้างขึ้นใหม่ได้ทันที รอ4ชั่วโมงและพยายามที่จะปรับเปลี่ยนนโยบายที่สร้างขึ้นใหม่อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="7d523-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="7d523-105">นโยบายการประชุมจะใช้ในการควบคุมลักษณะการทำงานที่มีให้กับผู้เข้าร่วมประชุมสำหรับการประชุมที่ได้รับการจัดกำหนดการไว้ในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="7d523-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="7d523-106">คุณลักษณะบางอย่างของนโยบายการประชุมอาจไม่ได้ถูกนำมาใช้ในศูนย์การจัดการทีมยัง (เหล่านี้จะมีป้ายชื่อว่า "เร็วๆนี้" ในเอกสารประกอบ)</span><span class="sxs-lookup"><span data-stu-id="7d523-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="7d523-107">ในกรณีนี้หรือถ้าคุณได้รับข้อผิดพลาดเช่น "เราไม่สามารถปรับปรุงนโยบายในขณะนี้แต่ลองอีกครั้งในภายหลัง" ในศูนย์ผู้ดูแลของ Microsoft ทีมเราขอแนะนำให้คุณใช้ PowerShell เพื่อสร้างหรือปรับเปลี่ยนนโยบายการประชุมของทีม</span><span class="sxs-lookup"><span data-stu-id="7d523-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="7d523-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการประชุมดูทรัพยากรต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7d523-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="7d523-109">เมื่อต้องการเรียนรู้เกี่ยวกับการสร้างนโยบายให้ทำการเปลี่ยนแปลงและกำหนดผู้ใช้ให้กับนโยบายโปรดดู[ที่จัดการนโยบายการประชุมในทีม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="7d523-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="7d523-110">เมื่อต้องการทำการเปลี่ยนแปลงนโยบายโดยใช้ cmdlets PowerShell ให้ดูที่[ภาพรวมของทีม PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="7d523-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="7d523-111">คุณจำเป็นต้องใช้[Skype สำหรับโมดูล PowerShell ธุรกิจ](https://www.microsoft.com/download/details.aspx?id=39366)สำหรับทีมนโยบายการประชุม</span><span class="sxs-lookup"><span data-stu-id="7d523-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="7d523-112">ตรวจทานการ[\*-CsTeamsMeetingPolicy cmdlet ของเอกสาร](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="7d523-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

