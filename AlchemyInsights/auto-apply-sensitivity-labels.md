---
title: การนำป้ายความลับไปใช้โดยอัตโนมัติ
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
ms.openlocfilehash: 8f316ad92ff31e28c3b3ffd25f25bd03ee159380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715184"
---
# <a name="auto-apply-sensitivity-labels"></a><span data-ttu-id="51e65-102">การนำป้ายความลับไปใช้โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="51e65-102">Auto-apply sensitivity labels</span></span>

<span data-ttu-id="51e65-103">ป้ายชื่อความลับสามารถนำไปใช้กับเนื้อหาของผู้ใช้ด้วยตนเองหรือคุณสามารถกำหนดค่าให้นำไปใช้กับเนื้อหาโดยอัตโนมัติได้</span><span class="sxs-lookup"><span data-stu-id="51e65-103">Sensitivity labels can be manually applied to content by users, or you can configure them to be automatically applied to content.</span></span>

<span data-ttu-id="51e65-104">การนำป้ายความลับไปใช้โดยอัตโนมัติเอาความต้องการในการฝึกอบรมผู้ใช้เกี่ยวกับวิธีการจัดประเภทเนื้อหาและจำเป็นต้องแจ้งให้พวกเขาทราบเกี่ยวกับการกำหนดค่านโยบาย</span><span class="sxs-lookup"><span data-stu-id="51e65-104">Automatically applying sensitivity labels removes the need to train users on how to classify content and the need to notify them of policy configurations.</span></span>

<span data-ttu-id="51e65-105">เมื่อต้องการนำป้ายชื่อไปใช้โดยอัตโนมัติจำเป็นต้องมีสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="51e65-105">To apply labels automatically, the following is required:</span></span>

- <span data-ttu-id="51e65-106">การสมัครใช้งานข้อมูล Azure Protection P2</span><span class="sxs-lookup"><span data-stu-id="51e65-106">Azure Information Protection P2 subscription</span></span>
- [<span data-ttu-id="51e65-107">ดาวน์โหลดและติดตั้งไคลเอ็นต์การติดตามข้อมูล Azure unified</span><span class="sxs-lookup"><span data-stu-id="51e65-107">Download and install the Azure Information Protection unified labeling client</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/install-unifiedlabelingclient-app)

<span data-ttu-id="51e65-108">เรากำลังทำงานกับการสนับสนุนพื้นเมืองที่ไม่จำเป็นต้องมีการป้องกันข้อมูล Azure ที่รวมกันไคลเอ็นต์การติดฉลากในอนาคต</span><span class="sxs-lookup"><span data-stu-id="51e65-108">We're working on native support that won't require the Azure Information Protection unified labeling client in the future.</span></span>

<span data-ttu-id="51e65-109">ในปัจจุบัน Windows เท่านั้นที่สนับสนุนไคลเอ็นต์การติดฉลากแบบครบวงจร</span><span class="sxs-lookup"><span data-stu-id="51e65-109">Currently, only Windows supports the unified labeling client.</span></span>  <span data-ttu-id="51e65-110">ฟีเจอร์นี้ยังไม่ได้รับการสนับสนุนบน Mac, iOS และ Android</span><span class="sxs-lookup"><span data-stu-id="51e65-110">The feature is not yet supported on Mac, iOS and Android.</span></span>

<span data-ttu-id="51e65-111">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับป้ายชื่อความลับและนำไปใช้กับเนื้อหาโดยอัตโนมัติให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="51e65-111">For more information on sensitivity labels and applying them automatically to content,  see:</span></span>

- [<span data-ttu-id="51e65-112">ภาพรวมของป้ายชื่อความลับ</span><span class="sxs-lookup"><span data-stu-id="51e65-112">Overview of sensitivity labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)
- [<span data-ttu-id="51e65-113">นำป้ายความลับไปใช้กับเนื้อหาโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="51e65-113">Apply a sensitivity label to content automatically</span></span>](https://docs.microsoft.com/office365/securitycompliance/apply_sensitivity_label_automatically)