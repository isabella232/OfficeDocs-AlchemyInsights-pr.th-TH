---
title: ไอคอนปฏิทินที่ไม่แสดงในไคลเอ็นต์ของทีม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: f30cd5bda62756cf6b912ed150b4e59e7ca4d85d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684717"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="71a48-102">ไอคอนปฏิทินที่ไม่แสดงในไคลเอ็นต์ของทีม</span><span class="sxs-lookup"><span data-stu-id="71a48-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="71a48-103">แท็บปฏิทินในทีมจำเป็นต้องมีสิทธิ์การเข้าถึงกล่องจดหมาย Exchange ผ่านทางเว็บเซอร์วิส Exchange</span><span class="sxs-lookup"><span data-stu-id="71a48-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="71a48-104">กล่องจดหมาย Exchange สามารถออนไลน์หรือภายในองค์กรได้</span><span class="sxs-lookup"><span data-stu-id="71a48-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="71a48-105">สำหรับผู้ใช้ออนไลน์ที่ไม่เห็นแท็บปฏิทินตรวจสอบให้แน่ใจว่า[ได้รับสิทธิ์การใช้งานสำหรับกล่องจดหมาย Exchange Online และกล่องจดหมายถูกเปิดใช้งาน](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="71a48-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="71a48-106">ถ้าผู้ใช้มีกล่องจดหมายที่ถูกต้องใน Exchange Online แต่ยังไม่สามารถเห็นแท็บปฏิทินคุณอาจพบปัญหาเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="71a48-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="71a48-107">ใช้ตัว [วิเคราะห์การเชื่อมต่อระยะไกลของ microsoft](https://testconnectivity.microsoft.com/) และเรียกใช้การ **ทดสอบการเชื่อมต่อบริการเว็บ microsoft Exchange** สำหรับผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="71a48-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="71a48-108">ในที่สุดการตรวจสอบ[แอปทีม–นโยบายการตั้งค่าแอป](https://admin.teams.microsoft.com/policies/app-setup)เพื่อให้แน่ใจว่าแอปปฏิทินไม่ได้ถูกเอาออกจากนโยบายที่ถูกนำไปใช้กับผู้ใช้ (ที่เป็นไปได้มากที่สุดคือส่วน**กลาง (ค่าเริ่มต้นทั้งองค์กร)**</span><span class="sxs-lookup"><span data-stu-id="71a48-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="71a48-109">ถ้าผู้ใช้ของคุณได้รับการ homed ภายในองค์กรคุณจำเป็นต้องยืนยันการกำหนดค่าไฮบริดของคุณที่มีสุขภาพดี</span><span class="sxs-lookup"><span data-stu-id="71a48-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="71a48-110">ใช้ [ตัวช่วยสร้างการกำหนดค่าแบบไฮบริดเพื่อ](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) แก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="71a48-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="71a48-111">โปรดทราบว่า[ทีมจำเป็นต้องมี Exchange ๒๐๑๖ CU3 หรือสูงกว่า](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)</span><span class="sxs-lookup"><span data-stu-id="71a48-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
