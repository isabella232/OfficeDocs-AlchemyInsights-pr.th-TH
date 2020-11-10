---
title: การใช้ Giphys ในการสนทนาของทีม
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982575"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="5ef3c-102">การใช้ Giphys ในการสนทนาของทีม</span><span class="sxs-lookup"><span data-stu-id="5ef3c-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="5ef3c-103">การเข้าถึง Giphys ในทีมการสนทนาจะถูกเปิดใช้งานตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="5ef3c-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="5ef3c-104">**ใน** ฐานะผู้ดูแลระบบคุณสามารถควบคุมได้ว่า Giphys จะพร้อมใช้งานสำหรับผู้ใช้โดย [การตั้งค่านโยบายการส่งข้อความ](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings)และตรวจสอบให้แน่ใจว่า **ใช้ Giphys ในการสนทนา**</span><span class="sxs-lookup"><span data-stu-id="5ef3c-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="5ef3c-105">ถ้า GIFs ไม่ทำงานตามที่คาดไว้ในการสนทนาของทีมให้ตรวจสอบดังนี้</span><span class="sxs-lookup"><span data-stu-id="5ef3c-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="5ef3c-106">[นโยบายการส่งข้อ](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams)ความจำเป็นต้องมีการอนุญาตให้ Giphys</span><span class="sxs-lookup"><span data-stu-id="5ef3c-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="5ef3c-107">เมื่อต้องการตรวจสอบโดยใช้ cmdlet ของ PowerShell ให้ใช้วิธีต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="5ef3c-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="5ef3c-108">ตรวจสอบว่าคุณสามารถ [จัดการทีมด้วย PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)ได้</span><span class="sxs-lookup"><span data-stu-id="5ef3c-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="5ef3c-109">เรียกใช้คำสั่ง PowerShell [ได้รับ-CsTeamsMessagingPolicy-ข้อมูลประจำตัว-ส่วนกลาง](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps)และตรวจสอบว่า **AllowGiphy** ถูกตั้งค่าเป็น **TRUE**</span><span class="sxs-lookup"><span data-stu-id="5ef3c-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="5ef3c-110">ถ้า **AllowGiphy** ถูกตั้งค่าเป็น **FALSE** ให้เรียกใช้คำสั่ง PowerShell ชุดต่อไปนี้ [-CsTeamsMessagingPolicy-ข้อมูลประจำตัว AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="5ef3c-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="5ef3c-111">จำเป็นต้องเปิดใช้งานการ[เชื่อมต่อ](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences)ที่ไม่จำเป็นต้องเปิดใช้งานเพื่ออนุญาตการเข้าถึง URL Giphy</span><span class="sxs-lookup"><span data-stu-id="5ef3c-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="5ef3c-112">ถ้าคุณมีนโยบายการส่งข้อความหลายทีมที่กำหนดค่าสำหรับผู้เช่าของคุณคุณสามารถกำหนดข้อมูลเฉพาะตัวของนโยบายที่กำหนดให้กับผู้ใช้ที่ได้รับผลกระทบที่มีคำสั่ง PowerShell ที่ [ได้รับการ CsOnlineUser-ข้อมูลประจำตัว](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> เลือก TeamsMessagingPolicy</span><span class="sxs-lookup"><span data-stu-id="5ef3c-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
