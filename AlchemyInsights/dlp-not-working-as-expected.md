---
title: DLP ไม่ใช้งานตามที่คาดไว้
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707829"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="8dc5f-102">DLP ไม่ใช้งานตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="8dc5f-102">DLP not working as expected</span></span>

<span data-ttu-id="8dc5f-103">**สิ่ง** สําคัญ: ในระหว่างช่วงเวลาที่ไม่มีประวัติการเป็นประวัติการเหล่านี้ เราอยู่ในระหว่างขั้นตอนเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานอยู่โปรดเยี่ยมชมการปรับปรุงฟีเจอร์ชั่วคราวของ [SharePoint Online](https://aka.ms/ODSPAdjustments) เพื่อดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="8dc5f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="8dc5f-104">**การตั้งค่า DLP**</span><span class="sxs-lookup"><span data-stu-id="8dc5f-104">**Setting up DLP**</span></span>

<span data-ttu-id="8dc5f-105">คุณมีปัญหากับการป้องกันการ **สูญหายของข้อมูล (DLP)** ใน Office 365 ไม่เป็นไปตามที่คาดไว้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="8dc5f-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="8dc5f-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span><span class="sxs-lookup"><span data-stu-id="8dc5f-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="8dc5f-107">นโยบาย DLP ช่วยให้คุณสามารถระบุและปกป้องข้อมูลที่ละเอียดอ่อนในองค์กรของคุณได้</span><span class="sxs-lookup"><span data-stu-id="8dc5f-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="8dc5f-108">เมื่อต้องการตั้งค่านโยบาย DLP ให้ใช้ [ข้อมูล](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)ที่นี่</span><span class="sxs-lookup"><span data-stu-id="8dc5f-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="8dc5f-109">**นโยบาย DLP มีลักษณะอย่างไร**</span><span class="sxs-lookup"><span data-stu-id="8dc5f-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="8dc5f-110">เมื่อใช้ชนิดข้อมูล **ที่ละเอียดอ่อนที่มีอยู่แล้วภายในใน** ศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย นโยบาย DLP จะค้นหารูปแบบและองค์ประกอบเฉพาะเมื่อตรวจหาชนิดที่เป็นความลับเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="8dc5f-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="8dc5f-111">**ชนิดข้อมูลที่ละเอียดอ่อนที่มีอยู่แล้วภายใน**</span><span class="sxs-lookup"><span data-stu-id="8dc5f-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="8dc5f-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="8dc5f-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="8dc5f-113">**ชนิดข้อมูลที่เป็นความลับแบบเอง**</span><span class="sxs-lookup"><span data-stu-id="8dc5f-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="8dc5f-114">ถ้าคุณพยายามสร้างชนิดข้อมูลที่มีความอ่อนไหวแบบเอง ให้ใช้บทความต่อไปนี้เพื่อดูข้อมูลเกี่ยวกับวิธีการสร้างชนิดที่เป็นความลับที่แบบปรับแต่งเอง:[สร้างชนิดข้อมูลที่ละเอียดอ่อนแบบเอง](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="8dc5f-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="8dc5f-115">**ทดสอบนโยบาย DLP**</span><span class="sxs-lookup"><span data-stu-id="8dc5f-115">**Test a DLP policy**</span></span>

<span data-ttu-id="8dc5f-116">เมื่อต้องการทดสอบข้อมูลของคุณด้วยชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายในหรือแบบจําเป็น ให้ใช้ตัวเลือก **ชนิดการทดสอบ\*\*\*\*ภายใต้ชนิดข้อมูล**  >  **ที่ละเอียดอ่อนของ** การจัดประเภท</span><span class="sxs-lookup"><span data-stu-id="8dc5f-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="8dc5f-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="8dc5f-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="8dc5f-118">**รายงาน**</span><span class="sxs-lookup"><span data-stu-id="8dc5f-118">**Reports**</span></span>
  
- <span data-ttu-id="8dc5f-119">รับข้อมูลเชิงลึกด้วย [รายงาน DLP](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="8dc5f-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="8dc5f-120">ดูรายละเอียดเฉพาะของเหตุการณ์ที่มี[รายงานเหตุการณ์](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="8dc5f-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
