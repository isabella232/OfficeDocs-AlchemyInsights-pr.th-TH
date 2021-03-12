---
title: ใช้ป้ายชื่อระดับความลับโดยอัตโนมัติ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1737"
- "9000181"
ms.openlocfilehash: fb05213b7b1efecbabc3e25f6c4587b0d303f783
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707253"
---
# <a name="auto-apply-sensitivity-labels"></a><span data-ttu-id="f81ec-102">ใช้ป้ายชื่อระดับความลับโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="f81ec-102">Auto-apply sensitivity labels</span></span>

<span data-ttu-id="f81ec-103">ป้ายชื่อระดับความลับสามารถถูกปรับใช้กับเนื้อหาด้วยตนเองโดยผู้ใช้ หรือคุณสามารถกําหนดค่าให้ใช้กับเนื้อหาโดยอัตโนมัติได้</span><span class="sxs-lookup"><span data-stu-id="f81ec-103">Sensitivity labels can be manually applied to content by users, or you can configure them to be automatically applied to content.</span></span>

<span data-ttu-id="f81ec-104">การใช้ป้ายชื่อระดับความลับโดยอัตโนมัติจะลบความต้องฝึกอบรมผู้ใช้เกี่ยวกับวิธีการจัดประเภทเนื้อหาและความต้องแจ้งให้พวกเขาทราบเกี่ยวกับการกําหนดค่านโยบาย</span><span class="sxs-lookup"><span data-stu-id="f81ec-104">Automatically applying sensitivity labels removes the need to train users on how to classify content and the need to notify them of policy configurations.</span></span>

<span data-ttu-id="f81ec-105">เมื่อต้องการใช้ป้ายชื่อโดยอัตโนมัติ สิ่งต่อไปนี้จะต้องใช้:</span><span class="sxs-lookup"><span data-stu-id="f81ec-105">To apply labels automatically, the following is required:</span></span>

- <span data-ttu-id="f81ec-106">การสมัครใช้งาน Azure Information Protection P2</span><span class="sxs-lookup"><span data-stu-id="f81ec-106">Azure Information Protection P2 subscription</span></span>
- [<span data-ttu-id="f81ec-107">ดาวน์โหลดและติดตั้งไคลเอ็นต์ป้ายผนึกส่วนรวมของ Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="f81ec-107">Download and install the Azure Information Protection unified labeling client</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/install-unifiedlabelingclient-app)

<span data-ttu-id="f81ec-108">เราพยายามอย่างเต็มที่ที่จะไม่ต้องใช้ไคลเอ็นต์การติดป้ายรวมของ Azure Information Protection ในอนาคต</span><span class="sxs-lookup"><span data-stu-id="f81ec-108">We're working on native support that won't require the Azure Information Protection unified labeling client in the future.</span></span>

<span data-ttu-id="f81ec-109">ในขณะนี้ เฉพาะ Windows เท่านั้นที่สนับสนุนไคลเอ็นต์ป้ายผนึกแบบรวม</span><span class="sxs-lookup"><span data-stu-id="f81ec-109">Currently, only Windows supports the unified labeling client.</span></span>  <span data-ttu-id="f81ec-110">ฟีเจอร์นี้ยังไม่ได้รับการสนับสนุนบน Mac, iOS และ Android</span><span class="sxs-lookup"><span data-stu-id="f81ec-110">The feature is not yet supported on Mac, iOS and Android.</span></span>

<span data-ttu-id="f81ec-111">ดูข้อมูลเพิ่มเติมเกี่ยวกับป้ายชื่อระดับความลับและปรับใช้กับเนื้อหาโดยอัตโนมัติที่:</span><span class="sxs-lookup"><span data-stu-id="f81ec-111">For more information on sensitivity labels and applying them automatically to content,  see:</span></span>

- [<span data-ttu-id="f81ec-112">ภาพรวมของป้ายระดับความลับ</span><span class="sxs-lookup"><span data-stu-id="f81ec-112">Overview of sensitivity labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)
- [<span data-ttu-id="f81ec-113">ใช้ป้ายชื่อระดับความลับกับเนื้อหาโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="f81ec-113">Apply a sensitivity label to content automatically</span></span>](https://docs.microsoft.com/microsoft-365/compliance/apply-sensitivity-label-automatically)