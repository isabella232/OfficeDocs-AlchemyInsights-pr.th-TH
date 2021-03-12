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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733868"
---
# <a name="11-call-recording"></a><span data-ttu-id="27bf5-102">การบันทึกการโทรแบบ 1:1</span><span class="sxs-lookup"><span data-stu-id="27bf5-102">1:1 call recording</span></span>

<span data-ttu-id="27bf5-103">ผู้ดูแลระบบต้องจัดการทันทีเพื่ออนุญาตให้ผู้ใช้บันทึกการโทรแบบ 1:1 ได้ต่อไป</span><span class="sxs-lookup"><span data-stu-id="27bf5-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="27bf5-104">ตั้งแต่วันที่ 12 เมษายน 2021 เราจะเริ่มบังคับใช้ตัวเลือกนโยบายการโทรของ Teams ใหม่ *AllowCloudRecordingForCalls*</span><span class="sxs-lookup"><span data-stu-id="27bf5-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="27bf5-105">ขณะนี้ความสามารถในการบันทึกการโทรแบบ 1:1 จะถูกควบคุมโดยตัวเลือก *AllowCloudRecording* ในนโยบายการประชุม Teams</span><span class="sxs-lookup"><span data-stu-id="27bf5-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="27bf5-106">ถ้าผู้ใช้ของคุณได้รับอนุญาตให้บันทึกการประชุม Teams พวกเขาจะสามารถบันทึกการโทรแบบ 1:1 ได้</span><span class="sxs-lookup"><span data-stu-id="27bf5-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="27bf5-107">ถ้าคุณต้องการบล็อกผู้ใช้ทั้งหมดจากการบันทึกการโทรแบบ 1:1 คุณไม่ต้องการที่จะหยุดการใดๆ</span><span class="sxs-lookup"><span data-stu-id="27bf5-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="27bf5-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span><span class="sxs-lookup"><span data-stu-id="27bf5-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="27bf5-109">การเปลี่ยนแปลงนี้อยู่ในโพสต์ของศูนย์ข้อความต่อไปนี้: (อัปเดต) บทนํานโยบายการบันทึกการโทรแบบ[1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)เมื่อต้องการตั้งค่าตัวเลือกนโยบายการโทรของ Teams คุณต้องใช้[Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="27bf5-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="27bf5-110">**เมื่อต้องการเปิดใช้งานการบันทึกการโทรในการโทรแบบ 1:1 ให้** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="27bf5-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="27bf5-111">**เมื่อต้องการปิดใช้งานการบันทึกการโทรในการโทรแบบ 1:1 ให้** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="27bf5-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

