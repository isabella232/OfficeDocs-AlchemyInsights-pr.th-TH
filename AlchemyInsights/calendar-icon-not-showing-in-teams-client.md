---
title: ไอคอนปฏิทินไม่แสดงในไคลเอ็นต์ Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932382"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="30f63-102">ไอคอนปฏิทินไม่แสดงในไคลเอ็นต์ Teams</span><span class="sxs-lookup"><span data-stu-id="30f63-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="30f63-103">แท็บปฏิทินในทีมต้องเข้าถึงกล่องจดหมาย Exchange ผ่านทางเว็บเซอร์วิสของอัตราแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="30f63-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="30f63-104">กล่องจดหมาย Exchange สามารถออนไลน์หรือในสถาน</span><span class="sxs-lookup"><span data-stu-id="30f63-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="30f63-105">สําหรับผู้ใช้ออนไลน์ที่ไม่เห็นแท็บปฏิทินตรวจสอบให้แน่ใจว่า[พวกเขาจะได้รับอนุญาตสําหรับกล่องจดหมาย Exchange แบบออนไลน์ และกล่องจดหมายถูกเปิดใช้งาน](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="30f63-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="30f63-106">ถ้าผู้ใช้มีกล่องจดหมายที่ถูกต้องใน Exchange แบบออนไลน์ แต่ยังคงไม่สามารถเห็นแท็บปฏิทินคุณอาจประสบปัญหาเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="30f63-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="30f63-107">ใช้[ตัววิเคราะห์การเชื่อมต่อระยะไกลของ Microsoft](https://testconnectivity.microsoft.com/)และเรียกใช้**การทดสอบการเชื่อมต่อบริการเว็บ Exchange Microsoft**สําหรับผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="30f63-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="30f63-108">สุดท้ายตรวจสอบ[แอปทีม - นโยบายการตั้งค่าแอป](https://admin.teams.microsoft.com/policies/app-setup)เพื่อให้แน่ใจว่าแอปปฏิทินไม่ได้ถูกลบออกจากนโยบายที่นําไปใช้กับผู้ใช้ (ส่วนใหญ่น่าจะเป็น**แบบส่วนกลาง (ค่าเริ่มต้นทั้งองค์กร)**</span><span class="sxs-lookup"><span data-stu-id="30f63-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="30f63-109">หากผู้ใช้ของคุณ homed ในสถานที่ คุณจําเป็นต้องยืนยันว่าการกําหนดค่าไฮบริดของคุณมีสุขภาพดี</span><span class="sxs-lookup"><span data-stu-id="30f63-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="30f63-110">ใช้[ตัวช่วยสร้างการตั้งค่าคอนฟิกไฮบริดสลี](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)การแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="30f63-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="30f63-111">โปรดทราบว่า[ทีมต้องการ CU3 2016 ของ Exchange หรือสูงกว่า](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)</span><span class="sxs-lookup"><span data-stu-id="30f63-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
