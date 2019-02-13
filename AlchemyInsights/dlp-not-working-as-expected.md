---
title: DLP ไม่ทำงานตามที่คาดไว้
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 1e5ff53d903a14064147621df0a883152c32eff5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919675"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="f29e8-102">DLP ไม่ทำงานตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="f29e8-102">DLP not working as expected</span></span>


<span data-ttu-id="f29e8-p101">คุณกำลังมีปัญหากับ**การป้องกันการสูญเสียข้อมูล (DLP)** ใน Office 365 ไม่ทำงานตามที่คาดไว้หรือไม่ ถ้าเป็นเช่นนั้น ให้แน่ใจ ว่า**นโยบาย DLP**ของคุณถูกตั้งค่าอย่างถูกต้อง ว่า ข้อมูลของคุณประกอบด้วยอะไร**นโยบาย DLP**จะค้นหาเมื่อมีการประเมิน</span><span class="sxs-lookup"><span data-stu-id="f29e8-p101">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected? If so, make sure that your **DLP policy** is setup correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span> 
  
 <span data-ttu-id="f29e8-105">**การตั้งค่า DLP:**</span><span class="sxs-lookup"><span data-stu-id="f29e8-105">**Setting up DLP:**</span></span>
  
<span data-ttu-id="f29e8-p102">นโยบาย DLP ช่วยให้คุณสามารถระบุ และปกป้องข้อมูลที่สำคัญในองค์กรของคุณ เมื่อต้องการตั้งค่านโยบาย DLP ใช้รายละเอียด[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)</span><span class="sxs-lookup"><span data-stu-id="f29e8-p102">DLP policies allows you to identify and protect sensitive information in your organization. To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="f29e8-108">**นโยบาย DLP สิ่งที่ค้นหา:**</span><span class="sxs-lookup"><span data-stu-id="f29e8-108">**What DLP policies look for:**</span></span>
  
<span data-ttu-id="f29e8-109">เมื่อใช้**ชนิดของข้อมูลที่สำคัญที่มีอยู่แล้วภาย**ใน Office 365 ปลอดภัยและปฏิบัติตามกฎระเบียบศูนย์ นโยบาย DLP ค้นหาเฉพาะรูปแบบและองค์ประกอบเมื่อตรวจพบชนิดเหล่านี้เป็นความลับ</span><span class="sxs-lookup"><span data-stu-id="f29e8-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span> 
  
- <span data-ttu-id="f29e8-110">**ชนิดของข้อมูลที่สำคัญอยู่แล้วภายใน:**</span><span class="sxs-lookup"><span data-stu-id="f29e8-110">**Built-in Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="f29e8-111">สำหรับข้อมูลเกี่ยวกับชนิดสำคัญมีอยู่ภายในและอะไรนโยบาย DLP ค้นหาเมื่อทำการตรวจหาชนิดใบสำคัญ ดู:[ชนิดข้อมูลที่เป็นความลับค้นหา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="f29e8-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
    
- <span data-ttu-id="f29e8-112">**ชนิดข้อมูลแบบกำหนดเองที่สำคัญ:**</span><span class="sxs-lookup"><span data-stu-id="f29e8-112">**Custom Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="f29e8-113">ถ้าคุณกำลังพยายามสร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญ ใช้บทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับวิธีการสร้างชนิดสำคัญแบบกำหนดเอง:[สร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญ](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="f29e8-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>
    
 <span data-ttu-id="f29e8-114">**รายงาน:**</span><span class="sxs-lookup"><span data-stu-id="f29e8-114">**Reports:**</span></span>
  
- <span data-ttu-id="f29e8-115">รับความเข้าใจข้อมูลที่สำคัญด้วย[DLP รายงาน](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="f29e8-115">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>
    
- <span data-ttu-id="f29e8-116">ดูรายละเอียดเฉพาะของเหตุการณ์ที่มีการ[รายงานเหตุการณ์](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="f29e8-116">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
    

