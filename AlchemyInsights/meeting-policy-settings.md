---
title: การตั้งค่านโยบายการประชุม
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825462"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="d5db2-102">จัดการนโยบายการประชุมใน Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d5db2-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="d5db2-103">**หมายเหตุ: อาจต้องใช้เวลาถึง 24 ชั่วโมงเพื่อให้การเปลี่ยนแปลงนโยบายมีผลกับผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="d5db2-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="d5db2-104">คุณอาจไม่สามารถเปลี่ยนแปลงนโยบายที่สร้างขึ้นใหม่ได้ทันที รอ 4 ชั่วโมง และพยายามปรับเปลี่ยนนโยบายที่สร้างขึ้นใหม่อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="d5db2-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="d5db2-105">นโยบายการประชุมจะถูกใช้เพื่อควบคุมฟีเจอร์ต่างๆ ที่พร้อมใช้งานกับผู้เข้าร่วมประชุมของการประชุมที่จัดเวลาโดยผู้ใช้ในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="d5db2-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="d5db2-106">ฟีเจอร์บางอย่างของนโยบายการประชุมอาจไม่ถูกปรับใช้ในศูนย์การจัดการ Teams (มีป้ายชื่อ "เร็วๆ นี้" ในเอกสารประกอบ)</span><span class="sxs-lookup"><span data-stu-id="d5db2-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="d5db2-107">ในกรณีนี้ หรือถ้าคุณได้รับข้อผิดพลาด เช่น "เราไม่สามารถอัปเดตนโยบายได้ในขณะนี้ แต่โปรดลองอีกครั้งในภายหลัง" ในศูนย์การจัดการ Microsoft Teams เราขอแนะนนะให้คุณใช้ PowerShell ในการสร้างหรือปรับเปลี่ยนนโยบายการประชุม Teams</span><span class="sxs-lookup"><span data-stu-id="d5db2-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="d5db2-108">ดูข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการประชุมที่แหล่งข้อมูลต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="d5db2-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="d5db2-109">เมื่อต้องการเรียนรู้เกี่ยวกับการสร้างนโยบาย การเปลี่ยนแปลง และการกําหนดนโยบายให้กับผู้ใช้ ให้ดู[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="d5db2-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="d5db2-110">เมื่อต้องการเปลี่ยนแปลงนโยบายโดยใช้ cmdlet ของ PowerShell ให้ดู[ภาพรวมของ Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="d5db2-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="d5db2-111">คุณต้องใช้มอดู [ล PowerShell ของ Skype for Business](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams นโยบายการประชุม</span><span class="sxs-lookup"><span data-stu-id="d5db2-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="d5db2-112">ตรวจทาน [เอกสาร cmdlets \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) เพื่อดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="d5db2-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

