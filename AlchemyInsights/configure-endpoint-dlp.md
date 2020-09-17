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
ms.openlocfilehash: 406bc40fbe8a6306a2f74506ef1daf70b37283d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812134"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="8fcc5-102">กำหนดค่าจุดสิ้นสุด DLP</span><span class="sxs-lookup"><span data-stu-id="8fcc5-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="8fcc5-103">Microsoft จุดสิ้นสุด DLP ช่วยให้คุณสามารถขยายความสามารถในการป้องกัน DLP และการตรวจสอบความสามารถของข้อมูลที่สำคัญบนอุปกรณ์ Windows 10</span><span class="sxs-lookup"><span data-stu-id="8fcc5-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="8fcc5-104">หลังจากที่อุปกรณ์ onboarded เข้าสู่การจัดการอุปกรณ์แล้วคุณสามารถสร้างนโยบาย DLP เพื่อบังคับใช้การดำเนินการป้องกันในรายการได้</span><span class="sxs-lookup"><span data-stu-id="8fcc5-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="8fcc5-105">กิจกรรม Explorer สามารถใช้เพื่อตรวจสอบกิจกรรมสำหรับรายการที่มีความสำคัญได้</span><span class="sxs-lookup"><span data-stu-id="8fcc5-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="8fcc5-106">สำหรับข้อมูลเพิ่มเติมให้ดูที่[อุปกรณ์ปฐมนิเทศลงในการจัดการอุปกรณ์](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)</span><span class="sxs-lookup"><span data-stu-id="8fcc5-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="8fcc5-107">เมื่อต้องการเริ่มต้นใช้งาน DLP สำหรับจุดสิ้นสุดให้ทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="8fcc5-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="8fcc5-108">ตรวจสอบให้แน่ใจว่าคุณมีสิทธิ์การใช้งาน SKU/การสมัครใช้งานที่เหมาะสม</span><span class="sxs-lookup"><span data-stu-id="8fcc5-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="8fcc5-109">สำหรับข้อมูลเพิ่มเติมให้ดูที่สิทธิ์การใช้งาน [SKU/การสมัคร](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)ใช้งาน</span><span class="sxs-lookup"><span data-stu-id="8fcc5-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="8fcc5-110">ตรวจสอบสิทธิ์ที่จำเป็นในการเปิดใช้งานการจัดการอุปกรณ์ให้เข้าถึงหน้าปฐมนิเทศหรือเปิด/ปิดการตรวจสอบอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="8fcc5-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="8fcc5-111">สำหรับข้อมูลเพิ่มเติมให้ดูที่[สิทธิ์](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)</span><span class="sxs-lookup"><span data-stu-id="8fcc5-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="8fcc5-112">อุปกรณ์ Onboard ลงในการจัดการอุปกรณ์โดยการติดตามขั้นตอนอุปกรณ์ปฐมนิเทศ</span><span class="sxs-lookup"><span data-stu-id="8fcc5-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="8fcc5-113">ถ้าคุณไม่พบตัวเลือกอุปกรณ์ปฐมนิเทศ (preview) ภายใต้  **การตั้งค่าการ**ปฏิบัติตามข้อบังคับ M365 ให้ยืนยันว่าคุณมีสิทธิ์การใช้งานที่เหมาะสมและสิทธิ์ที่อ้างอิงด้านบน</span><span class="sxs-lookup"><span data-stu-id="8fcc5-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="8fcc5-114">สำหรับข้อมูลเพิ่มเติมให้ดูที่[อุปกรณ์ปฐมนิเทศ](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)</span><span class="sxs-lookup"><span data-stu-id="8fcc5-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="8fcc5-115">สร้างนโยบาย DLP เพื่อป้องกันรายการที่เป็นความลับของคุณ</span><span class="sxs-lookup"><span data-stu-id="8fcc5-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="8fcc5-116">สำหรับข้อมูลเพิ่มเติมให้ดูที่ [สถานการณ์สมมติของนโยบาย DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)ของจุดสิ้นสุด</span><span class="sxs-lookup"><span data-stu-id="8fcc5-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="8fcc5-117">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ DLP จุดสิ้นสุดของ Microsoft ให้ดูที่[เรียนรู้เกี่ยวกับการป้องกันการสูญหายของข้อมูลจุดสิ้นสุดของ microsoft ๓๖๕ (การแสดงตัวอย่าง)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)</span><span class="sxs-lookup"><span data-stu-id="8fcc5-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>