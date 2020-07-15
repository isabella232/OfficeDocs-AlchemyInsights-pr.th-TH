---
title: ปัญหาเกี่ยวกับเครื่องออนบอร์ด
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141836"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="cd546-102">ปัญหาเกี่ยวกับเครื่องออนบอร์ด</span><span class="sxs-lookup"><span data-stu-id="cd546-102">Issues with onboarding machines</span></span>

<span data-ttu-id="cd546-103">คุณอาจมีปัญหากับเครื่องออนบอร์ดไปยังบริการ MDATP</span><span class="sxs-lookup"><span data-stu-id="cd546-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="cd546-104">ถ้าคุณสามารถเข้าถึงเครื่องผู้ใช้ ให้ทําตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="cd546-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="cd546-105">ดาวน์โหลดเครื่องมือการวินิจฉัย[ตัววิเคราะห์การเชื่อมต่อไคลเอ็นต์](https://aka.ms/mdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="cd546-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="cd546-106">สารสกัดและเรียกใช้ MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="cd546-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="cd546-107">ค้นหาล็อกการวินิจฉัยในโฟลเดอร์ที่เรียกว่า MDATPClientAnalyzerResult โฟลเดอร์เดียวกันที่เครื่องมือวิเคราะห์ถูกดาวน์โหลด</span><span class="sxs-lookup"><span data-stu-id="cd546-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="cd546-108">ตรวจสอบแฟ้มบันทึก MDATPClientAnalyzer.txt เพื่อค้นหาปัญหาการตั้งค่าการเชื่อมต่อหรือพร็อกซีอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="cd546-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>