---
title: DLP ไม่ทํางานตามที่คาดไว้
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932641"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="e60ff-102">DLP ไม่ทํางานตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="e60ff-102">DLP not working as expected</span></span>

<span data-ttu-id="e60ff-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="e60ff-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e60ff-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="e60ff-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e60ff-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="e60ff-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e60ff-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="e60ff-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e60ff-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="e60ff-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e60ff-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="e60ff-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="e60ff-109">**การตั้งค่า DLP**</span><span class="sxs-lookup"><span data-stu-id="e60ff-109">**Setting up DLP**</span></span>

<span data-ttu-id="e60ff-110">คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ใน Office 365 ไม่ทํางานตามที่คาดไว้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="e60ff-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="e60ff-111">ถ้าเป็นเช่นนั้น โปรดตรวจสอบให้แน่ใจว่า**นโยบาย DLP**ของคุณถูกตั้งค่าอย่างถูกต้อง และว่า ข้อมูลของคุณประกอบด้วย**นโยบาย DLP**กําลังค้นหาเมื่อมีการประเมิน</span><span class="sxs-lookup"><span data-stu-id="e60ff-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="e60ff-112">นโยบาย DLP ช่วยให้คุณสามารถระบุและปกป้องข้อมูลที่ละเอียดอ่อนในองค์กรของคุณได้</span><span class="sxs-lookup"><span data-stu-id="e60ff-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="e60ff-113">เมื่อต้องการตั้งค่านโยบาย DLP ให้ใช้ข้อมูล[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)</span><span class="sxs-lookup"><span data-stu-id="e60ff-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="e60ff-114">**สิ่งที่นโยบาย DLP มองหา**</span><span class="sxs-lookup"><span data-stu-id="e60ff-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="e60ff-115">เมื่อใช้**ชนิดข้อมูลที่สําคัญที่มีอยู่แล้วภายใน**ใน Office 365 Security and Compliance Center นโยบาย DLP จะค้นหารูปแบบและองค์ประกอบเฉพาะเมื่อตรวจพบชนิดที่ละเอียดอ่อนเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="e60ff-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="e60ff-116">**ชนิดข้อมูลที่ละเอียดอ่อนในตัว**</span><span class="sxs-lookup"><span data-stu-id="e60ff-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="e60ff-117">สําหรับข้อมูลเกี่ยวกับชนิดที่ละเอียดอ่อนที่มีอยู่แล้วภายใน และนโยบาย DLP จะค้นหาอะไรเมื่อตรวจหาชนิดอ่อนไหว ให้ดูที่:[ชนิดของข้อมูลที่ละเอียดอ่อนจะค้นหา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="e60ff-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="e60ff-118">**ชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="e60ff-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="e60ff-119">ถ้าคุณกําลังพยายามสร้างชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง ให้ใช้บทความต่อไปนี้สําหรับข้อมูลเกี่ยวกับวิธีการสร้างชนิดที่ละเอียดอ่อนแบบกําหนดเอง:[สร้างชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="e60ff-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="e60ff-120">**ทดสอบนโยบาย DLP**</span><span class="sxs-lookup"><span data-stu-id="e60ff-120">**Test a DLP policy**</span></span>

<span data-ttu-id="e60ff-121">เมื่อต้องการทดสอบข้อมูลของคุณด้วยชนิดข้อมูลที่ละเอียดอ่อนในตัวหรือแบบกําหนดเอง ให้ใช้ตัวเลือก**ประเภทการทดสอบ**ภายใต้**Classifications** > **ชนิดข้อมูลที่ละเอียดอ่อน**</span><span class="sxs-lookup"><span data-stu-id="e60ff-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="e60ff-122">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ทดสอบชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="e60ff-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="e60ff-123">**รายงาน**</span><span class="sxs-lookup"><span data-stu-id="e60ff-123">**Reports**</span></span>
  
- <span data-ttu-id="e60ff-124">รับข้อมูลเชิงลึกของข้อมูลที่ละเอียดอ่อนด้วย[รายงาน DLP](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="e60ff-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="e60ff-125">ดูรายละเอียดเฉพาะของเหตุการณ์ที่มี[รายงานเหตุการณ์](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="e60ff-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
