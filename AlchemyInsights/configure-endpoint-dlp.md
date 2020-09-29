---
title: กำหนดค่าจุดสิ้นสุด DLP
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
ms.openlocfilehash: d0363d6bdecdb266a5f4a3a14bd496ede6bb9931
ms.sourcegitcommit: 76b147af688f0dc39878a913a050c0e56af054a8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/29/2020
ms.locfileid: "48305462"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="35c70-102">กำหนดค่าจุดสิ้นสุด DLP</span><span class="sxs-lookup"><span data-stu-id="35c70-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="35c70-103">Microsoft จุดสิ้นสุด DLP ช่วยให้คุณสามารถขยายความสามารถในการป้องกัน DLP และการตรวจสอบความสามารถของข้อมูลที่สำคัญบนอุปกรณ์ Windows 10</span><span class="sxs-lookup"><span data-stu-id="35c70-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="35c70-104">หลังจากที่อุปกรณ์ onboarded เข้าสู่การจัดการอุปกรณ์แล้วคุณสามารถสร้างนโยบาย DLP เพื่อบังคับใช้การดำเนินการป้องกันในรายการได้</span><span class="sxs-lookup"><span data-stu-id="35c70-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="35c70-105">กิจกรรม Explorer สามารถใช้เพื่อตรวจสอบกิจกรรมสำหรับรายการที่มีความสำคัญได้</span><span class="sxs-lookup"><span data-stu-id="35c70-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="35c70-106">สำหรับข้อมูลเพิ่มเติมให้ดูที่[อุปกรณ์ปฐมนิเทศลงในการจัดการอุปกรณ์](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)</span><span class="sxs-lookup"><span data-stu-id="35c70-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="35c70-107">เมื่อต้องการเริ่มต้นใช้งาน DLP สำหรับจุดสิ้นสุดให้ทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="35c70-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="35c70-108">ตรวจสอบให้แน่ใจว่าคุณมีสิทธิ์การใช้งาน SKU/การสมัครใช้งานที่เหมาะสม</span><span class="sxs-lookup"><span data-stu-id="35c70-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="35c70-109">สำหรับข้อมูลเพิ่มเติมให้ดูที่สิทธิ์การใช้งาน [SKU/การสมัคร](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)ใช้งาน</span><span class="sxs-lookup"><span data-stu-id="35c70-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="35c70-110">ตรวจสอบสิทธิ์ที่จำเป็นในการเปิดใช้งานการจัดการอุปกรณ์ให้เข้าถึงหน้าปฐมนิเทศหรือเปิด/ปิดการตรวจสอบอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="35c70-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="35c70-111">สำหรับข้อมูลเพิ่มเติมให้ดูที่[สิทธิ์](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)</span><span class="sxs-lookup"><span data-stu-id="35c70-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="35c70-112">อุปกรณ์ Onboard ลงในการจัดการอุปกรณ์โดยการติดตามขั้นตอนอุปกรณ์ปฐมนิเทศ</span><span class="sxs-lookup"><span data-stu-id="35c70-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="35c70-113">ถ้าคุณไม่พบตัวเลือกอุปกรณ์ปฐมนิเทศ (preview) ภายใต้  **การตั้งค่าการ**ปฏิบัติตามข้อบังคับ M365 ให้ยืนยันว่าคุณมีสิทธิ์การใช้งานที่เหมาะสมและสิทธิ์ที่อ้างอิงด้านบน</span><span class="sxs-lookup"><span data-stu-id="35c70-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="35c70-114">สำหรับข้อมูลเพิ่มเติมให้ดูที่[อุปกรณ์ปฐมนิเทศ](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)</span><span class="sxs-lookup"><span data-stu-id="35c70-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="35c70-115">สร้างนโยบาย DLP เพื่อป้องกันรายการที่เป็นความลับของคุณ</span><span class="sxs-lookup"><span data-stu-id="35c70-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="35c70-116">สำหรับข้อมูลเพิ่มเติมให้ดูที่ [สถานการณ์สมมติของนโยบาย DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)ของจุดสิ้นสุด</span><span class="sxs-lookup"><span data-stu-id="35c70-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="35c70-117">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ DLP จุดสิ้นสุดของ Microsoft ให้ดูที่[เรียนรู้เกี่ยวกับการป้องกันการสูญหายของข้อมูลจุดสิ้นสุดของ microsoft ๓๖๕ (การแสดงตัวอย่าง)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)</span><span class="sxs-lookup"><span data-stu-id="35c70-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="35c70-118">**ขั้นตอนการรวบรวมข้อมูลที่สำคัญถ้าจำเป็นต้องมีการสนับสนุน:**</span><span class="sxs-lookup"><span data-stu-id="35c70-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="35c70-119">ดาวน์โหลด MDATP การแสดงตัวอย่างตัววิเคราะห์ไคลเอ็นต์จาก [http://aka.ms/betamdatpanalyzer](http://aka.ms/betamdatpanalyzer "http://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="35c70-119">Download MDATP Client Analyzer Preview from [http://aka.ms/betamdatpanalyzer](http://aka.ms/betamdatpanalyzer "http://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="35c70-120">เรียกใช้เครื่องมือในฐานะผู้ดูแลระบบจากหน้าต่าง cmd:</span><span class="sxs-lookup"><span data-stu-id="35c70-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="35c70-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd – t</span><span class="sxs-lookup"><span data-stu-id="35c70-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="35c70-122">เมื่อได้รับพร้อมท์ด้วย "ใส่จำนวนนาทีในการรวบรวมการสืบค้นกลับ:" ให้ใส่จำนวนนาทีที่จำเป็นต้องใช้ในการเรียกใช้สถานการณ์สมมติ</span><span class="sxs-lookup"><span data-stu-id="35c70-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="35c70-123">เรียกใช้สถานการณ์สมมติ</span><span class="sxs-lookup"><span data-stu-id="35c70-123">Run the scenario</span></span>

<span data-ttu-id="35c70-124">การรวบรวมผลลัพธ์ของไฟล์ Zip ที่จะมอบให้กับตัวแทนฝ่ายสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="35c70-124">Collect the Zip file output to be given to the Support agent.</span></span>
