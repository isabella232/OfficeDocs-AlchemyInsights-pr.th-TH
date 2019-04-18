---
title: ใช้ป้ายชื่อในระดับความลับโดยอัตโนมัติ
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 65d359f9826e689963cfe5e83b37227cbadd526b
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909620"
---
# <a name="auto-apply-sensitivity-labels"></a><span data-ttu-id="5ed65-102">ใช้ป้ายชื่อในระดับความลับโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="5ed65-102">Auto-apply sensitivity labels</span></span>

<span data-ttu-id="5ed65-103">ป้ายชื่อของระดับความสำคัญสามารถเป็น mannually ที่นำไปใช้กับเนื้อหาที่ผู้ใช้ หรือคุณสามารถกำหนดค่าเหล่านี้สามารถนำไปใช้กับเนื้อหาโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="5ed65-103">Sensitivity labels can be mannually applied to content by users, or you can configure them to be automatically applied to content.</span></span>

<span data-ttu-id="5ed65-104">ป้ายชื่อระดับความลับที่นำไปใช้โดยอัตโนมัติเอาจำเป็นในการฝึกอบรมผู้ใช้เกี่ยวกับวิธีการจัดประเภทเนื้อหาและจำเป็นต้องแจ้งให้ทราบการตั้งค่าคอนฟิกนโยบายเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="5ed65-104">Automatically applying sensitivity labels removes the need to train users on how to classify content and the need to notify them of policy configurations.</span></span>

<span data-ttu-id="5ed65-105">เมื่อต้องการใช้ป้ายชื่อโดยอัตโนมัติ ต่อไปนี้จำเป็นต้องมี:</span><span class="sxs-lookup"><span data-stu-id="5ed65-105">To apply labels automatically, the following is required:</span></span>

- <span data-ttu-id="5ed65-106">บอกรับเป็นสมาชิก P2 ป้องกันข้อมูล azure</span><span class="sxs-lookup"><span data-stu-id="5ed65-106">Azure Information Protection P2 subscription</span></span>
- [<span data-ttu-id="5ed65-107">ดาวน์โหลดและติดตั้งการป้องกันข้อมูล Azure รวมจับกลุ่มไคลเอนต์</span><span class="sxs-lookup"><span data-stu-id="5ed65-107">Download and install the Azure Information Protection unified labeling client</span></span>](https://docs.microsoft.com/en-us/azure/information-protection/rms-client/install-unifiedlabelingclient-app)

<span data-ttu-id="5ed65-108">เรากำลังทำงานบนการสนับสนุนท้องถิ่นที่ไม่จำเป็นต้องมีการป้องกันข้อมูล Azure ประกอบการ labeling ไคลเอนต์ในอนาคต</span><span class="sxs-lookup"><span data-stu-id="5ed65-108">We're working on native support that won't require the Azure Information Protection unified labeling client in the future.</span></span>

<span data-ttu-id="5ed65-109">ในปัจจุบัน Windows เท่านั้นสนับสนุนไคลเอ็นต์ labeling ประกอบการ</span><span class="sxs-lookup"><span data-stu-id="5ed65-109">Currently, only Windows supports the unified labeling client.</span></span>  <span data-ttu-id="5ed65-110">คุณลักษณะไม่ได้สนับสนุนบน Mac, iOS และ Android</span><span class="sxs-lookup"><span data-stu-id="5ed65-110">The feature is not yet supported on Mac, iOS and Android.</span></span>

<span data-ttu-id="5ed65-111">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับความลับป้ายและนำไปใช้โดยอัตโนมัติกับเนื้อหา ดู:</span><span class="sxs-lookup"><span data-stu-id="5ed65-111">For more information on sensitivity labels and applying them automatically to content,  see:</span></span>

- [<span data-ttu-id="5ed65-112">ภาพรวมของป้ายความไว</span><span class="sxs-lookup"><span data-stu-id="5ed65-112">Overview of sensitivity labels</span></span>](https://docs.microsoft.com/en-us/office365/securitycompliance/sensitivity-labels)
- [<span data-ttu-id="5ed65-113">ป้ายชื่อที่มีความอ่อนไหวนำไปใช้กับเนื้อหาโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="5ed65-113">Apply a sensitivity label to content automatically</span></span>](https://docs.microsoft.com/en-us/office365/securitycompliance/apply_sensitivity_label_automatically)