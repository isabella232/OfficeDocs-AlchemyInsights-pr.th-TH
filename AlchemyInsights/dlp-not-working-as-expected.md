---
title: DLP ไม่ทำงานตามที่คาดไว้
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
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679712"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="726c7-102">DLP ไม่ทำงานตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="726c7-102">DLP not working as expected</span></span>

<span data-ttu-id="726c7-103">**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="726c7-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="726c7-104">**การตั้งค่า DLP**</span><span class="sxs-lookup"><span data-stu-id="726c7-104">**Setting up DLP**</span></span>

<span data-ttu-id="726c7-105">คุณมีปัญหาเกี่ยวกับการ **ป้องกันการสูญหายของข้อมูล (DLP)** ใน Office ๓๖๕ไม่ทำงานตามที่คาดไว้ใช่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="726c7-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="726c7-106">ถ้าเป็นเช่นนั้นตรวจสอบให้แน่ใจว่า **นโยบาย dlp** ของคุณได้รับการตั้งค่าอย่างถูกต้องและข้อมูลของคุณมีสิ่งที่ **นโยบาย dlp** กำลังค้นหาเมื่อมีการประเมิน</span><span class="sxs-lookup"><span data-stu-id="726c7-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="726c7-107">นโยบาย DLP ช่วยให้คุณสามารถระบุและปกป้องข้อมูลที่สำคัญในองค์กรของคุณได้</span><span class="sxs-lookup"><span data-stu-id="726c7-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="726c7-108">เมื่อต้องการตั้งค่านโยบาย DLP ให้ใช้ข้อมูล[ต่อไปนี้](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)</span><span class="sxs-lookup"><span data-stu-id="726c7-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="726c7-109">**นโยบาย DLP ใดที่ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="726c7-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="726c7-110">เมื่อใช้ **ชนิดข้อมูลที่มีอยู่แล้วภาย** ในในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย DLP ให้มองหารูปแบบและองค์ประกอบเฉพาะเมื่อตรวจหาชนิดที่มีความสำคัญเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="726c7-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="726c7-111">**ชนิดข้อมูลที่มีความสำคัญที่มีอยู่แล้วภายใน**</span><span class="sxs-lookup"><span data-stu-id="726c7-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="726c7-112">สำหรับข้อมูลเกี่ยวกับชนิดที่มีอยู่แล้วภายในและนโยบาย DLP จะมีลักษณะอย่างไรเมื่อตรวจหาชนิดที่มีความสำคัญให้ดูที่:[ชนิดข้อมูลที่มีความสำคัญคืออะไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="726c7-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="726c7-113">**ชนิดข้อมูลที่เป็นความลับแบบกำหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="726c7-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="726c7-114">ถ้าคุณกำลังพยายามสร้างชนิดข้อมูลที่มีความสำคัญแบบกำหนดเองให้ใช้บทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับวิธีการสร้างชนิดที่มีความสำคัญแบบกำหนดเอง: การ[สร้างชนิดข้อมูลที่เป็นความลับแบบกำหนดเอง](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="726c7-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="726c7-115">**ทดสอบนโยบาย DLP**</span><span class="sxs-lookup"><span data-stu-id="726c7-115">**Test a DLP policy**</span></span>

<span data-ttu-id="726c7-116">เมื่อต้องการทดสอบข้อมูลของคุณด้วยชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายในหรือแบบกำหนดเองให้ใช้ตัวเลือก**ชนิดการทดสอบ\*\*\*\*ภายใต้การจัดประเภท**  >  **ข้อมูล**ที่มีความสำคัญ</span><span class="sxs-lookup"><span data-stu-id="726c7-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="726c7-117">สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[ทดสอบชนิดข้อมูลที่เป็นความลับแบบกำหนดเอง](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="726c7-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="726c7-118">**รายงาน**</span><span class="sxs-lookup"><span data-stu-id="726c7-118">**Reports**</span></span>
  
- <span data-ttu-id="726c7-119">รับข้อมูลเชิงลึกของข้อมูลที่มีความสำคัญกับ [รายงาน DLP](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="726c7-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="726c7-120">ดูรายละเอียดเฉพาะของเหตุการณ์ที่มี[รายงานเหตุการณ์](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="726c7-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
