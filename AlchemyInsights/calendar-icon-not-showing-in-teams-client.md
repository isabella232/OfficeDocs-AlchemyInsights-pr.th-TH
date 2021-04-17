---
title: ไอคอนปฏิทินไม่แสดงในไคลเอ็นต์ Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819972"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="869df-102">ไอคอนปฏิทินไม่แสดงในไคลเอ็นต์ Teams</span><span class="sxs-lookup"><span data-stu-id="869df-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="869df-103">แท็บ ปฏิทิน ใน Teams ต้องมีสิทธิ์เข้าถึงกล่องจดหมาย Exchange ผ่านทาง Exchange Web Services</span><span class="sxs-lookup"><span data-stu-id="869df-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="869df-104">กล่องจดหมาย Exchange สามารถเป็นแบบออนไลน์หรือภายในองค์กรได้</span><span class="sxs-lookup"><span data-stu-id="869df-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="869df-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="869df-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="869df-106">ถ้าผู้ใช้มีกล่องจดหมายที่ถูกต้องใน Exchange Online แต่ยังคงไม่เห็นแท็บ ปฏิทิน คุณอาจประสบปัญหาเกี่ยวกับเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="869df-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="869df-107">ใช้ [ตัววิเคราะห์การเชื่อมต่อระยะไกลของ](https://testconnectivity.microsoft.com/) ไมโครซอฟท์ และเรียกใช้ **การทดสอบการเชื่อมต่อบริการเว็บ Microsoft Exchange** ให้กับผู้ใช้ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="869df-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="869df-108">สุดท้าย ตรวจสอบแอป [Teams –](https://admin.teams.microsoft.com/policies/app-setup)นโยบายการตั้งค่าแอปเพื่อให้แน่ใจว่าแอปปฏิทินยังไม่ได้ถูกลบออกจากนโยบายที่ปรับใช้กับผู้ใช้ (ส่วนใหญ่คือส่วนกลาง **(ค่าเริ่มต้นทั่วทั้งองค์กร)**</span><span class="sxs-lookup"><span data-stu-id="869df-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="869df-109">ถ้าผู้ใช้ของคุณอยู่ในระบบภายในองค์กร คุณต้องยืนยันว่าการกําหนดค่าแบบไฮบริดของคุณสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="869df-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="869df-110">ใช้ตัวช่วยสร้าง [การกําหนดค่าแบบ](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) ไฮบริดเพื่อแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="869df-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="869df-111">โปรดทราบว่า[Teams ต้องใช้ Exchange 2016 CU3 หรือสูงกว่า](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)</span><span class="sxs-lookup"><span data-stu-id="869df-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
