---
title: DLP ไม่ทํางานตามที่คาดไว้
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: efb4a19f345fe6b8a1e8bb72abeba4a923c05777
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704432"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="f3649-102">DLP ไม่ทํางานตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="f3649-102">DLP not working as expected</span></span>

<span data-ttu-id="f3649-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="f3649-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="f3649-104">**การตั้งค่า DLP**</span><span class="sxs-lookup"><span data-stu-id="f3649-104">**Setting up DLP**</span></span>

<span data-ttu-id="f3649-105">คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ใน Office 365 ไม่ทํางานตามที่คาดไว้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="f3649-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="f3649-106">ถ้าเป็นเช่นนั้น โปรดตรวจสอบให้แน่ใจว่า**นโยบาย DLP**ของคุณถูกตั้งค่าอย่างถูกต้อง และว่า ข้อมูลของคุณประกอบด้วย**นโยบาย DLP**กําลังค้นหาเมื่อมีการประเมิน</span><span class="sxs-lookup"><span data-stu-id="f3649-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="f3649-107">นโยบาย DLP ช่วยให้คุณสามารถระบุและปกป้องข้อมูลที่ละเอียดอ่อนในองค์กรของคุณได้</span><span class="sxs-lookup"><span data-stu-id="f3649-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="f3649-108">เมื่อต้องการตั้งค่านโยบาย DLP ให้ใช้ข้อมูล[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)</span><span class="sxs-lookup"><span data-stu-id="f3649-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="f3649-109">**สิ่งที่นโยบาย DLP มองหา**</span><span class="sxs-lookup"><span data-stu-id="f3649-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="f3649-110">เมื่อใช้**ชนิดข้อมูลที่สําคัญในตัว**ในศูนย์ความปลอดภัยและการปฏิบัติตามกฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="f3649-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="f3649-111">**ชนิดข้อมูลที่ละเอียดอ่อนในตัว**</span><span class="sxs-lookup"><span data-stu-id="f3649-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="f3649-112">สําหรับข้อมูลเกี่ยวกับชนิดที่ละเอียดอ่อนที่มีอยู่แล้วภายใน และนโยบาย DLP จะค้นหาอะไรเมื่อตรวจหาชนิดอ่อนไหว ให้ดูที่:[ชนิดของข้อมูลที่ละเอียดอ่อนจะค้นหา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="f3649-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="f3649-113">**ชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="f3649-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="f3649-114">ถ้าคุณกําลังพยายามสร้างชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง ให้ใช้บทความต่อไปนี้สําหรับข้อมูลเกี่ยวกับวิธีการสร้างชนิดที่ละเอียดอ่อนแบบกําหนดเอง:[สร้างชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="f3649-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="f3649-115">**ทดสอบนโยบาย DLP**</span><span class="sxs-lookup"><span data-stu-id="f3649-115">**Test a DLP policy**</span></span>

<span data-ttu-id="f3649-116">เมื่อต้องการทดสอบข้อมูลของคุณด้วยชนิดข้อมูลที่ละเอียดอ่อนในตัวหรือแบบกําหนดเอง ให้ใช้ตัวเลือก**ประเภทการทดสอบ**ภายใต้**Classifications** > **ชนิดข้อมูลที่ละเอียดอ่อน**</span><span class="sxs-lookup"><span data-stu-id="f3649-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="f3649-117">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ทดสอบชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="f3649-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="f3649-118">**รายงาน**</span><span class="sxs-lookup"><span data-stu-id="f3649-118">**Reports**</span></span>
  
- <span data-ttu-id="f3649-119">รับข้อมูลเชิงลึกของข้อมูลที่ละเอียดอ่อนด้วย[รายงาน DLP](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="f3649-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="f3649-120">ดูรายละเอียดเฉพาะของเหตุการณ์ที่มี[รายงานเหตุการณ์](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="f3649-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
