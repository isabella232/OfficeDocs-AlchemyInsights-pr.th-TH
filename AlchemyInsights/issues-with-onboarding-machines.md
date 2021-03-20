---
title: ปัญหาเกี่ยวกับเครื่องออนบอร์ดไปยัง Microsoft Defender for Endpoints
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901586"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="240e2-102">ปัญหาเกี่ยวกับเครื่องออนบอร์ดไปยัง Microsoft Defender for Endpoints</span><span class="sxs-lookup"><span data-stu-id="240e2-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="240e2-103">คุณอาจมีปัญหากับเครื่องออนบอร์ดลงในบริการ MDE</span><span class="sxs-lookup"><span data-stu-id="240e2-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="240e2-104">ถ้าคุณสามารถเข้าถึงเครื่องของผู้ใช้ ปลายทาง ให้ปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="240e2-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="240e2-105">ดาวน์โหลดเวอร์ชันล่าสุดของเครื่องมือวินิจฉัย[ตัววิเคราะห์ไคลเอ็นต์ MDE](https://aka.ms/betamdeanalyzer)</span><span class="sxs-lookup"><span data-stu-id="240e2-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="240e2-106">คลิกขวาที่ **MDEClientAnalyzer.cmd** แล้วเลือก 'เรียกใช้ในฐานะผู้ดูแลระบบ'</span><span class="sxs-lookup"><span data-stu-id="240e2-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="240e2-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="240e2-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="240e2-108">ดูโฟลเดอร์ย่อยที่สร้างขึ้นที่ชื่อว่า **MDEClientAnalyzerResult** เพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="240e2-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="240e2-109">ถ้าต้องใช้แนวทางเพิ่มเติม ให้ติดต่อ [Microsoft Defender เพื่อรับการสนับสนุนเกี่ยวกับ](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) จุดสิ้นสุด และMDEClientAnalyzerResult.zipไฟล์สําหรับการวิเคราะห์</span><span class="sxs-lookup"><span data-stu-id="240e2-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
