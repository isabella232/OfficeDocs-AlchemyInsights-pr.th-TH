---
title: การกําหนดค่าจุดสิ้นสุด DLP
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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657948"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="fc2f3-102">การกําหนดค่าจุดสิ้นสุด DLP</span><span class="sxs-lookup"><span data-stu-id="fc2f3-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="fc2f3-103">Microsoft Endpoint DLP ช่วยให้คุณสามารถขยายการป้องกัน DLP และความสามารถในการตรวจสอบไปยังข้อมูลที่เป็นความลับWindows 10ต่างๆ</span><span class="sxs-lookup"><span data-stu-id="fc2f3-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="fc2f3-104">หลังจากที่อุปกรณ์ออนบอร์ดเข้าสู่การจัดการอุปกรณ์ คุณสามารถสร้างนโยบาย DLP เพื่อบังคับใช้การกระทกป้องกันบนรายการได้</span><span class="sxs-lookup"><span data-stu-id="fc2f3-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="fc2f3-105">สามารถใช้ Activity Explorer เพื่อตรวจสอบกิจกรรมของรายการที่ละเอียดอ่อนได้</span><span class="sxs-lookup"><span data-stu-id="fc2f3-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="fc2f3-106">ดูข้อมูลเพิ่มเติมได้ที่ [การออนบอร์ดอุปกรณ์ลงในการจัดการ](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="fc2f3-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="fc2f3-107">เมื่อต้องการเริ่มต้นใช้งานจุดสิ้นสุด DLP:</span><span class="sxs-lookup"><span data-stu-id="fc2f3-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="fc2f3-108">ตรวจสอบให้แน่ใจว่าคุณมีสิทธิ์การใช้งาน SKU/การสมัครใช้งานที่เหมาะสม</span><span class="sxs-lookup"><span data-stu-id="fc2f3-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="fc2f3-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="fc2f3-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="fc2f3-110">ตรวจสอบสิทธิ์ที่ต้องใช้เพื่อเปิดใช้งานการจัดการอุปกรณ์ เข้าถึงหน้าออนบอร์ด หรือเปิด/ปิดการตรวจสอบอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="fc2f3-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="fc2f3-111">ดูข้อมูลเพิ่มเติม [ที่](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)สิทธิ์</span><span class="sxs-lookup"><span data-stu-id="fc2f3-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="fc2f3-112">อุปกรณ์ Onboard ลงในการจัดการอุปกรณ์โดยปฏิบัติตามกระบวนการอุปกรณ์ Onboarding</span><span class="sxs-lookup"><span data-stu-id="fc2f3-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="fc2f3-113">ดูข้อมูลเพิ่มเติมได้ที่[อุปกรณ์ออนบอร์ด](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)</span><span class="sxs-lookup"><span data-stu-id="fc2f3-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="fc2f3-114">สร้างนโยบาย DLP เพื่อป้องกันรายการที่เป็นความลับของคุณ</span><span class="sxs-lookup"><span data-stu-id="fc2f3-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="fc2f3-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="fc2f3-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="fc2f3-116">For more information on the Microsoft Endpoint DLP, see [learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="fc2f3-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="fc2f3-117">**ขั้นตอนในการเก็บรวบรวมข้อมูลที่สําคัญ ถ้าต้องใช้การสนับสนุน:**</span><span class="sxs-lookup"><span data-stu-id="fc2f3-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="fc2f3-118">ดาวน์โหลด[ตัวอย่างตัววิเคราะห์ไคลเอ็นต์ MDATP](https://aka.ms/betamdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="fc2f3-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="fc2f3-119">เรียกใช้เครื่องมือในฐานะผู้ดูแลระบบจากหน้าต่าง cmd:</span><span class="sxs-lookup"><span data-stu-id="fc2f3-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="fc2f3-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="fc2f3-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="fc2f3-121">เมื่อได้รับพร้อมท์ **ให้ใส่จํานวนนาทีเพื่อรวบรวมการติดตาม:** ให้ใส่จํานวนนาทีที่ต้องใช้ในการเรียกใช้สถานการณ์สมมติ</span><span class="sxs-lookup"><span data-stu-id="fc2f3-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="fc2f3-122">เรียกใช้สถานการณ์สมมติ</span><span class="sxs-lookup"><span data-stu-id="fc2f3-122">Run the scenario.</span></span>

<span data-ttu-id="fc2f3-123">รวบรวมผลลัพธ์ไฟล์ Zip เพื่อให้กับตัวแทนฝ่ายสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="fc2f3-123">Collect the Zip file output to give to the Support agent.</span></span>
