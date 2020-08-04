---
title: ตั้งค่าคอนฟิก DLP ปลายทาง
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556033"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="9f8ce-102">ตั้งค่าคอนฟิก DLP ปลายทาง</span><span class="sxs-lookup"><span data-stu-id="9f8ce-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="9f8ce-103">Microsoft Endpoint DLP ช่วยให้คุณสามารถขยายความสามารถในการป้องกันและการตรวจสอบ DLP ไปยังข้อมูลที่ละเอียดอ่อนบนอุปกรณ์ Windows 10</span><span class="sxs-lookup"><span data-stu-id="9f8ce-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="9f8ce-104">หลังจากที่อุปกรณ์ถูกเปิดใช้งานในการจัดการอุปกรณ์แล้ว คุณสามารถสร้างนโยบาย DLP เพื่อบังคับใช้การดําเนินการป้องกันบนรายการได้</span><span class="sxs-lookup"><span data-stu-id="9f8ce-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="9f8ce-105">ตัวสํารวจกิจกรรมสามารถใช้ในการตรวจสอบกิจกรรมสําหรับรายการที่สําคัญ</span><span class="sxs-lookup"><span data-stu-id="9f8ce-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="9f8ce-106">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การเตรียมพร้อมอุปกรณ์เข้าสู่การจัดการอุปกรณ์](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)</span><span class="sxs-lookup"><span data-stu-id="9f8ce-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="9f8ce-107">เมื่อต้องการเริ่มต้นใช้งานปลายทาง DLP:</span><span class="sxs-lookup"><span data-stu-id="9f8ce-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="9f8ce-108">ตรวจสอบให้แน่ใจว่าคุณมีสิทธิ์การใช้งาน SKU/การสมัครใช้งานที่เหมาะสม</span><span class="sxs-lookup"><span data-stu-id="9f8ce-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="9f8ce-109">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การออกใบอนุญาต SKU/การสมัครใช้งาน](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)</span><span class="sxs-lookup"><span data-stu-id="9f8ce-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="9f8ce-110">ตรวจสอบสิทธิ์ที่จําเป็นเพื่อเปิดใช้งานการจัดการอุปกรณ์ เข้าถึงหน้าออนบอร์ด หรือเปิด/ปิดการตรวจสอบอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="9f8ce-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="9f8ce-111">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[สิทธิ์](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)</span><span class="sxs-lookup"><span data-stu-id="9f8ce-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="9f8ce-112">อุปกรณ์ออนบอร์ดเข้าสู่การจัดการอุปกรณ์โดยทําตามขั้นตอนอุปกรณ์ออนบอร์ด</span><span class="sxs-lookup"><span data-stu-id="9f8ce-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="9f8ce-113">หากคุณไม่มีตัวเลือกการเตรียมพร้อมสําหรับอุปกรณ์ (ดูตัวอย่าง) ภายใต้**การตั้งค่า**การปฏิบัติตามข้อกําหนด M365 ให้ยืนยันว่าคุณมีสิทธิ์การใช้งานและสิทธิ์ที่เหมาะสมที่อ้างอิงข้างต้น</span><span class="sxs-lookup"><span data-stu-id="9f8ce-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="9f8ce-114">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[อุปกรณ์ออนบอร์ด](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)</span><span class="sxs-lookup"><span data-stu-id="9f8ce-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="9f8ce-115">สร้างนโยบาย DLP เพื่อปกป้องรายการที่ละเอียดอ่อนของคุณ</span><span class="sxs-lookup"><span data-stu-id="9f8ce-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="9f8ce-116">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[สถานการณ์จําลองนโยบาย DLP ปลายทาง](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)</span><span class="sxs-lookup"><span data-stu-id="9f8ce-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="9f8ce-117">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับ Microsoft ปลายทาง DLP ดู[เรียนรู้เกี่ยวกับ Microsoft 365 ปลายทางข้อมูลสูญหายป้องกัน (ตัวอย่าง)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)</span><span class="sxs-lookup"><span data-stu-id="9f8ce-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>