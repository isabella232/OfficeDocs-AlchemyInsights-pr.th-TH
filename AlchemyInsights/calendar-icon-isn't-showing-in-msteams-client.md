---
title: ไอคอนปฏิทินไม่แสดงในไคลเอ็นต์ Microsoft team
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583929"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="a95ca-102">ไอคอนปฏิทินไม่แสดงในไคลเอ็นต์ Microsoft team</span><span class="sxs-lookup"><span data-stu-id="a95ca-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="a95ca-103">แท็บ **ปฏิทิน** ในทีมจำเป็นต้องมีสิทธิ์การเข้าถึงกล่องจดหมาย exchange ผ่านทางเว็บเซอร์วิส exchange</span><span class="sxs-lookup"><span data-stu-id="a95ca-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="a95ca-104">กล่องจดหมาย Exchange สามารถออนไลน์หรือภายในองค์กรได้</span><span class="sxs-lookup"><span data-stu-id="a95ca-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="a95ca-105">สำหรับผู้ใช้ออนไลน์ที่ไม่เห็นแท็บ **ปฏิทิน** ตรวจสอบให้แน่ใจว่า [ได้รับสิทธิ์การใช้งานสำหรับกล่องจดหมาย Exchange Online และกล่องจดหมายถูกเปิดใช้งาน](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="a95ca-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="a95ca-106">ถ้าผู้ใช้ของคุณ homed ภายในองค์กรคุณจำเป็นต้องยืนยันว่าการกำหนดค่าแบบไฮบริดของคุณมีสุขภาพดี</span><span class="sxs-lookup"><span data-stu-id="a95ca-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="a95ca-107">ใช้ [ตัวช่วยสร้างการกำหนดค่าแบบไฮบริดเพื่อ](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) แก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="a95ca-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="a95ca-108">โปรดทราบว่า[ทีมจำเป็นต้องมี Exchange ๒๐๑๖ CU3 หรือสูงกว่า](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)</span><span class="sxs-lookup"><span data-stu-id="a95ca-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="a95ca-109">สำหรับข้อมูลเพิ่มเติมและขั้นตอนการแก้ไขปัญหาให้ดูที่การ[แก้ไขปัญหาเกี่ยวกับทีม Microsoft และการโต้ตอบ Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)</span><span class="sxs-lookup"><span data-stu-id="a95ca-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
