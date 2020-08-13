---
title: แชนเนลส่วนตัว
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005457"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="e46aa-102">แชนเนลส่วนตัวในทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="e46aa-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="e46aa-103">แชนเนลส่วนตัวเป็นฟีเจอร์ใหม่ในทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="e46aa-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="e46aa-104">โปรดสังเกตว่าไม่สามารถแปลงแชนเนลส่วนตัวจากแชนเนลมาตรฐานหรือกลับกันได้</span><span class="sxs-lookup"><span data-stu-id="e46aa-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="e46aa-105">สำหรับรายละเอียดเกี่ยวกับแชนเนลส่วนตัวเช่นข้อมูลเกี่ยวกับการ[สร้างแชนเนลส่วนตัวและการเป็นสมาชิก](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership)และ[ไซต์ SharePoint ของแชนเนลส่วน](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)ตัวให้ดู[ที่แชนเนลส่วนตัวในทีม Microsoft](https://docs.microsoft.com/MicrosoftTeams/private-channels)</span><span class="sxs-lookup"><span data-stu-id="e46aa-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="e46aa-106">**หมายเหตุ:** เนื่องจากการกำหนดค่าสำหรับการเก็บรักษาข้อความของแชนเนลส่วนตัวยังไม่ได้รับการสนับสนุนผู้เช่าที่มีนโยบายการเก็บข้อมูลที่เปิดใช้งานจะไม่มีแชนเนลส่วนตัวที่เปิดใช้งานตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="e46aa-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="e46aa-107">คุณสามารถเปิดใช้งานแชนเนลส่วนตัวในศูนย์การจัดการทีมได้</span><span class="sxs-lookup"><span data-stu-id="e46aa-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="e46aa-108">นอกจากนี้โปรดทราบว่าขณะที่การเก็บรักษาข้อความของแชนเนลส่วนตัวไม่ได้รับการสนับสนุนการเก็บข้อมูลของไฟล์ที่แชร์ในแชนเนลส่วนตัวจะได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="e46aa-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="e46aa-109">**จำเป็นต้องมีเจ้าของทีมใหม่ใช่หรือไม่**</span><span class="sxs-lookup"><span data-stu-id="e46aa-109">**Need a new team owner?**</span></span>

<span data-ttu-id="e46aa-110">ถ้าเจ้าของแชนเนลส่วนตัวของคุณคุณสามารถเพิ่มเจ้าของทีมใหม่ผ่านทางทีม Powershell ได้</span><span class="sxs-lookup"><span data-stu-id="e46aa-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="e46aa-111">ไปที่[นี่](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6)เพื่อติดตั้งทีม Powershell</span><span class="sxs-lookup"><span data-stu-id="e46aa-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="e46aa-112">ต่อไปนี้คือ cmdlet ที่คุณจำเป็นต้องมี:</span><span class="sxs-lookup"><span data-stu-id="e46aa-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="e46aa-113">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับทีม Powershell ให้ดูที่[ภาพรวมของทีม powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="e46aa-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
