---
title: แก้ไขกฎการส่งผ่าน
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750572"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="919ab-102">แก้ไขกฎการส่งผ่าน</span><span class="sxs-lookup"><span data-stu-id="919ab-102">Fix transport rules</span></span>

<span data-ttu-id="919ab-103">กฎล>ล.ย.จดหมายแบบปรับแต่งเองมีผลต่อข้อความนี้</span><span class="sxs-lookup"><span data-stu-id="919ab-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="919ab-104">เมื่อต้องการตรวจทานกฎที่แน่นอน ให้ทต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="919ab-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="919ab-105">ในผลลัพธ์การส่ง **ภายใต้ข้อมูลเพิ่มเติม ให้** จด **GUID** หรือ **ชื่อ** นโยบาย</span><span class="sxs-lookup"><span data-stu-id="919ab-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="919ab-106">เปิดใช้ Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="919ab-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="919ab-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="919ab-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="919ab-108">เรียกใช้การสั่งนี้ (โดยใช้ GUID จากการส่งของคุณ):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="919ab-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="919ab-109">ตรวจทานรายละเอียดเพื่อดูเงื่อนไขที่กําหนดค่าแล้วที่ได้รับผลกระทบในข้อความ</span><span class="sxs-lookup"><span data-stu-id="919ab-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="919ab-110">เมื่อต้องการเรียนรู้เพิ่มเติม[ให้ดู Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="919ab-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
