---
title: ปัญหาเกี่ยวกับเครื่องปฐมนิเทศ
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
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676901"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="5ab48-102">ปัญหาเกี่ยวกับเครื่องปฐมนิเทศ</span><span class="sxs-lookup"><span data-stu-id="5ab48-102">Issues with onboarding machines</span></span>

<span data-ttu-id="5ab48-103">คุณอาจมีปัญหาเกี่ยวกับเครื่องปฐมนิเทศให้บริการ MDATP</span><span class="sxs-lookup"><span data-stu-id="5ab48-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="5ab48-104">ถ้าคุณสามารถเข้าถึงเครื่องของผู้ใช้ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="5ab48-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="5ab48-105">ดาวน์โหลดเครื่องมือการวินิจฉัยตัว[วิเคราะห์การเชื่อมต่อไคลเอ็นต์](https://aka.ms/mdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="5ab48-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="5ab48-106">แยกและเรียกใช้ MDATPAnalyzer</span><span class="sxs-lookup"><span data-stu-id="5ab48-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="5ab48-107">ค้นหาบันทึกการวินิจฉัยในโฟลเดอร์ที่ชื่อว่า MDATPClientAnalyzerResult โฟลเดอร์เดียวกันกับที่ดาวน์โหลดเครื่องมือตัววิเคราะห์</span><span class="sxs-lookup"><span data-stu-id="5ab48-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="5ab48-108">ตรวจทานไฟล์บันทึก MDATPClientAnalyzer.txt เพื่อค้นหาปัญหาการตั้งค่าการเชื่อมต่อหรือการตั้งค่าพร็อกซีของอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="5ab48-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>