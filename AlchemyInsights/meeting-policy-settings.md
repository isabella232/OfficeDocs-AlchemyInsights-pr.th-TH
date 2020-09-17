---
title: การตั้งค่านโยบายการประชุม
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794353"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="11c02-102">จัดการนโยบายการประชุมในทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="11c02-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="11c02-103">**หมายเหตุ: อาจใช้เวลาถึง24ชั่วโมงเพื่อให้การเปลี่ยนแปลงนโยบายมีผลต่อผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="11c02-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="11c02-104">คุณอาจไม่สามารถทำการเปลี่ยนแปลงไปยังนโยบายที่สร้างขึ้นใหม่ได้ทันที รอ4ชั่วโมงและพยายามปรับเปลี่ยนนโยบายที่สร้างขึ้นใหม่อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="11c02-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="11c02-105">นโยบายการประชุมจะถูกใช้ในการควบคุมฟีเจอร์ที่พร้อมใช้งานสำหรับผู้เข้าร่วมการประชุมสำหรับการประชุมที่จัดกำหนดการโดยผู้ใช้ในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="11c02-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="11c02-106">ฟีเจอร์บางอย่างของนโยบายการประชุมอาจไม่ถูกนำไปใช้ในศูนย์การจัดการทีมยัง (เหล่านี้จะมีป้ายชื่อว่า "มาเร็วๆนี้" ในเอกสารประกอบ)</span><span class="sxs-lookup"><span data-stu-id="11c02-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="11c02-107">ในกรณีนี้หรือถ้าคุณได้รับข้อผิดพลาดเช่น "เราไม่สามารถอัปเดตรายละเอียดได้ในขณะนี้แต่ลองอีกครั้งในภายหลัง" ในศูนย์การจัดการทีมของ Microsoft เราขอแนะนำให้คุณใช้ PowerShell เพื่อสร้างหรือปรับเปลี่ยนนโยบายการประชุมของทีม</span><span class="sxs-lookup"><span data-stu-id="11c02-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="11c02-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการประชุมให้ดูที่แหล่งข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="11c02-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="11c02-109">เมื่อต้องการเรียนรู้เกี่ยวกับการสร้างนโยบายการทำการเปลี่ยนแปลงและการกำหนดผู้ใช้ให้กับนโยบายให้ดูที่[จัดการนโยบายการประชุมในทีม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="11c02-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="11c02-110">เมื่อต้องการทำการเปลี่ยนแปลงนโยบายโดยใช้ cmdlet ของ PowerShell ให้ดูที่[ภาพรวมของทีม PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="11c02-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="11c02-111">คุณจำเป็นต้องใช้ [โมดูล PowerShell ของ Skype For business](https://www.microsoft.com/download/details.aspx?id=39366) สำหรับนโยบายการประชุมของทีม</span><span class="sxs-lookup"><span data-stu-id="11c02-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="11c02-112">ตรวจทาน [คู่มือ cmdlet ของ CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="11c02-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

