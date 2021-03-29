---
title: การกําหนดค่า DLP จุดสิ้นสุด
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402461"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="fe437-102">การกําหนดค่า DLP จุดสิ้นสุด</span><span class="sxs-lookup"><span data-stu-id="fe437-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="fe437-103">Microsoft Endpoint DLP ช่วยให้คุณสามารถขยายการป้องกัน DLP และความสามารถในการตรวจสอบข้อมูลที่ละเอียดอ่อนบนอุปกรณ์ Windows 10</span><span class="sxs-lookup"><span data-stu-id="fe437-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="fe437-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span><span class="sxs-lookup"><span data-stu-id="fe437-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="fe437-105">สามารถใช้ Activity Explorer เพื่อตรวจสอบกิจกรรมของรายการที่ละเอียดอ่อนได้</span><span class="sxs-lookup"><span data-stu-id="fe437-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="fe437-106">ดูข้อมูลเพิ่มเติมได้ที่ [การออนบอร์ดอุปกรณ์ในการจัดการ](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="fe437-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="fe437-107">เมื่อต้องการเริ่มต้นใช้งานจุดสิ้นสุด DLP:</span><span class="sxs-lookup"><span data-stu-id="fe437-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="fe437-108">ตรวจสอบให้แน่ใจว่าคุณมีสิทธิ์การใช้งาน SKU/การสมัครใช้งานที่เหมาะสม</span><span class="sxs-lookup"><span data-stu-id="fe437-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="fe437-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="fe437-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="fe437-110">ตรวจสอบสิทธิ์ที่ต้องใช้เพื่อเปิดใช้งานการจัดการอุปกรณ์ เข้าถึงหน้าการออนบอร์ด หรือเปิด/ปิดการตรวจสอบอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="fe437-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="fe437-111">ดูข้อมูลเพิ่มเติมได้ที่[สิทธิ์](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)</span><span class="sxs-lookup"><span data-stu-id="fe437-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="fe437-112">อุปกรณ์ออนบอร์ดเข้าสู่การจัดการอุปกรณ์โดยปฏิบัติตามกระบวนการอุปกรณ์แบบออนบอร์ด</span><span class="sxs-lookup"><span data-stu-id="fe437-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="fe437-113">ถ้าคุณไม่มีตัวเลือกการออนบอร์ดของอุปกรณ์ (ตัวอย่าง) ภายใต้การตั้งค่าการปฏิบัติตามนโยบายของ M365 ให้ยืนยันว่าคุณมีสิทธิ์การใช้งานและสิทธิ์ที่เหมาะสมที่อ้างอิงด้านบน</span><span class="sxs-lookup"><span data-stu-id="fe437-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="fe437-114">ดูข้อมูลเพิ่มเติมได้ที่[อุปกรณ์การออนบอร์ด](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)</span><span class="sxs-lookup"><span data-stu-id="fe437-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="fe437-115">สร้างนโยบาย DLP เพื่อป้องกันรายการที่เป็นความลับของคุณ</span><span class="sxs-lookup"><span data-stu-id="fe437-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="fe437-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="fe437-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="fe437-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="fe437-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="fe437-118">**ขั้นตอนในการเก็บรวบรวมข้อมูลที่สําคัญ ถ้าต้องใช้การสนับสนุน:**</span><span class="sxs-lookup"><span data-stu-id="fe437-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="fe437-119">ดาวน์โหลดตัวอย่างตัววิเคราะห์ไคลเอ็นต์ MDATP จาก [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="fe437-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="fe437-120">เรียกใช้เครื่องมือในฐานะผู้ดูแลระบบจากหน้าต่าง cmd:</span><span class="sxs-lookup"><span data-stu-id="fe437-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="fe437-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="fe437-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="fe437-122">เมื่อได้รับพร้อมท์ด้วย "ใส่จํานวนนาทีเพื่อรวบรวมการติดตาม: "ใส่จํานวนนาทีที่ต้องใช้เพื่อเรียกใช้สถานการณ์สมมติ</span><span class="sxs-lookup"><span data-stu-id="fe437-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="fe437-123">เรียกใช้สถานการณ์สมมติ</span><span class="sxs-lookup"><span data-stu-id="fe437-123">Run the scenario</span></span>

<span data-ttu-id="fe437-124">รวบรวมผลลัพธ์ไฟล์ Zip ที่จะให้กับตัวแทนฝ่ายสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="fe437-124">Collect the Zip file output to be given to the Support agent.</span></span>
