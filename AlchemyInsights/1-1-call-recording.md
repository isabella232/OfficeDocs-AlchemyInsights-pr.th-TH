---
title: การบันทึกการโทรแบบ 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702109"
---
# <a name="11-call-recording"></a><span data-ttu-id="bd2ad-102">การบันทึกการโทรแบบ 1:1</span><span class="sxs-lookup"><span data-stu-id="bd2ad-102">1:1 call recording</span></span>

<span data-ttu-id="bd2ad-103">ถ้า **ปุ่ม เริ่ม** การบันทึก เป็นสีเทาในการโทรแบบ 1:1 คุณจะต้องเปลี่ยนการตั้งค่านโยบายของผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="bd2ad-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="bd2ad-104">เมื่อต้องการตรวจสอบการตั้งค่านโยบาย ให้เรียกใช้ การวินิจฉัย ของผู้ใช้ที่มีผลกระทบโดยการพิมพ์ **Diag: Teams 1:1 การบันทึกการโทร** ด้านบน</span><span class="sxs-lookup"><span data-stu-id="bd2ad-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="bd2ad-105">ตั้งแต่วันที่ 31 พฤษภาคม 2021 เราจะเริ่มบังคับใช้นโยบายการโทรTeams *AllowCloudRecordingForCalls* ใหม่</span><span class="sxs-lookup"><span data-stu-id="bd2ad-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="bd2ad-106">ก่อนการเปลี่ยนแปลงนี้ การบันทึกการโทรแบบ 1:1 จะถูกควบคุมโดย *AllowCloudRecording Teams* นโยบายการประชุม</span><span class="sxs-lookup"><span data-stu-id="bd2ad-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="bd2ad-107">การเปลี่ยนแปลงนี้อยู่ในโพสต์ของศูนย์ข้อความ: [(อัปเดตแล้ว) 1:1 บทนํานโยบายการบันทึก](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)การโทร</span><span class="sxs-lookup"><span data-stu-id="bd2ad-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="bd2ad-108">*AllowCloudRecordingForCalls*   ตัวเลือกนโยบายการโทรถูกตั้งค่า **$False** ตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="bd2ad-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="bd2ad-109">ถ้าคุณต้องการบล็อกผู้ใช้ทั้งหมดไม่ให้บันทึกการโทรแบบ 1:1 คุณไม่ต้จะต้องการใดๆ</span><span class="sxs-lookup"><span data-stu-id="bd2ad-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="bd2ad-110">เมื่อต้องการเปิดใช้งานการบันทึกการโทรให้กับผู้ใช้ทั้งหมดในการโทรแบบ 1:1 [Teams PowerShell](/microsoftteams/teams-powershell-install)เพื่อเรียกใช้ cmdlet ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="bd2ad-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="bd2ad-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="bd2ad-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="bd2ad-112">อีกวิธีหนึ่งคือ คุณสามารถสร้างนโยบายใหม่และตั้งค่า **-AllowCloudRecordingForCalls** **เพื่อ$true** และกําหนดนโยบายนั้นให้กับผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="bd2ad-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="bd2ad-113">ดูข้อมูลเพิ่มเติมที่[1:1 การควบคุมนโยบายการบันทึกการโทร (เกือบเสร็จแล้ว!) ที่นี่](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)</span><span class="sxs-lookup"><span data-stu-id="bd2ad-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
