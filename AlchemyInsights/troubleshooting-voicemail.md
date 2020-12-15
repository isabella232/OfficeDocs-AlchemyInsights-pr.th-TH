---
title: 'การแก้ไขปัญหาข้อความเสียง '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679106"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="7277f-102">การแก้ไขปัญหาข้อความเสียง</span><span class="sxs-lookup"><span data-stu-id="7277f-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="7277f-103">ตรวจสอบให้แน่ใจว่ามีการใช้งานฟีเจอร์ที่ว่างไม่ว่าง</span><span class="sxs-lookup"><span data-stu-id="7277f-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="7277f-104">ถ้าไม่จำเป็นต้องใช้ฟีเจอร์นี้ในผู้ใช้นี้:</span><span class="sxs-lookup"><span data-stu-id="7277f-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="7277f-105">ไปที่[ศูนย์การจัดการทีม](https://admin.teams.microsoft.com/policies/calling)</span><span class="sxs-lookup"><span data-stu-id="7277f-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="7277f-106">บนรางด้านซ้ายนำทาง  >  **นโยบายการโทร** ด้วยเสียง  >  **จัดการนโยบาย** ในนโยบายการ **โทร**</span><span class="sxs-lookup"><span data-stu-id="7277f-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="7277f-107">เลือก **จัดการผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="7277f-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="7277f-108">การค้นหาผู้ใช้และการเปลี่ยนแปลงนโยบายการโทรไปยังที่ว่างไม่ว่าง **จะพร้อมใช้งานเมื่ออยู่ในการโทร\*\*\*\*ไปยัง**</span><span class="sxs-lookup"><span data-stu-id="7277f-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="7277f-109">คลิก **นำไปใช้**</span><span class="sxs-lookup"><span data-stu-id="7277f-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="7277f-110">การเปลี่ยนแปลงที่เกิดขึ้นกับนโยบายอาจใช้เวลาถึง24ชั่วโมงในการทำซ้ำ</span><span class="sxs-lookup"><span data-stu-id="7277f-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="7277f-111">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับฟีเจอร์นี้ให้ดูที่:[ไม่ว่างในการใช้งานว่างพร้อมใช้งานขณะอยู่ในการโทร](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call)</span><span class="sxs-lookup"><span data-stu-id="7277f-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
