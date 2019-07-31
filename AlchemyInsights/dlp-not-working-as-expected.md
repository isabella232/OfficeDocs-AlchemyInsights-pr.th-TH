---
title: DLP ไม่ทำงานตามที่คาดไว้
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
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941087"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="6864d-102">DLP ไม่ทำงานตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="6864d-102">DLP not working as expected</span></span>

<span data-ttu-id="6864d-103">คุณกำลังมีปัญหากับ**การป้องกันการสูญเสียข้อมูล (DLP)** ใน Office 365 ไม่ทำงานตามที่คาดไว้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="6864d-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="6864d-104">ถ้าเป็นเช่นนั้น ให้แน่ใจ ว่า**นโยบาย DLP**ของคุณถูกตั้งค่าอย่างถูกต้อง ว่า ข้อมูลของคุณประกอบด้วยอะไร**นโยบาย DLP**จะค้นหาเมื่อมีการประเมิน</span><span class="sxs-lookup"><span data-stu-id="6864d-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="6864d-105">**การตั้งค่า DLP**</span><span class="sxs-lookup"><span data-stu-id="6864d-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="6864d-106">นโยบาย DLP ช่วยให้คุณสามารถระบุ และปกป้องข้อมูลที่สำคัญในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="6864d-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="6864d-107">เมื่อต้องการตั้งค่านโยบาย DLP ใช้รายละเอียด[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)</span><span class="sxs-lookup"><span data-stu-id="6864d-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="6864d-108">**นโยบาย DLP ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="6864d-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="6864d-109">เมื่อใช้**ชนิดของข้อมูลที่สำคัญที่มีอยู่แล้วภาย**ใน Office 365 ปลอดภัยและปฏิบัติตามกฎระเบียบศูนย์ นโยบาย DLP ค้นหาเฉพาะรูปแบบและองค์ประกอบเมื่อตรวจพบชนิดเหล่านี้เป็นความลับ</span><span class="sxs-lookup"><span data-stu-id="6864d-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="6864d-110">**ชนิดของข้อมูลที่สำคัญอยู่แล้วภายใน**</span><span class="sxs-lookup"><span data-stu-id="6864d-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="6864d-111">สำหรับข้อมูลเกี่ยวกับชนิดสำคัญมีอยู่ภายในและอะไรนโยบาย DLP ค้นหาเมื่อทำการตรวจหาชนิดใบสำคัญ ดู:[ชนิดข้อมูลที่เป็นความลับค้นหา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="6864d-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="6864d-112">**ชนิดข้อมูลแบบกำหนดเองที่สำคัญ**</span><span class="sxs-lookup"><span data-stu-id="6864d-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="6864d-113">ถ้าคุณกำลังพยายามสร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญ ใช้บทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับวิธีการสร้างชนิดสำคัญแบบกำหนดเอง:[สร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญ](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="6864d-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="6864d-114">**ทดสอบนโยบาย DLP**</span><span class="sxs-lookup"><span data-stu-id="6864d-114">**Test a DLP policy**</span></span>

<span data-ttu-id="6864d-115">เมื่อต้องการทดสอบข้อมูลของคุณ มีชนิดข้อมูลที่เป็นความลับภายใน หรือแบบกำหนดเอง ให้ใช้ตัวเลือก**ชนิดของทดสอบ**ภายใต้**การจัดประเภท** > **ชนิดของข้อมูลที่เป็นความลับ**</span><span class="sxs-lookup"><span data-stu-id="6864d-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="6864d-116">สำหรับข้อมูลเพิ่มเติม ให้ดู[ชนิดของการทดสอบข้อมูลที่อ่อนไหวแบบกำหนดเอง](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="6864d-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="6864d-117">**รายงาน**</span><span class="sxs-lookup"><span data-stu-id="6864d-117">**Reports**</span></span>
  
- <span data-ttu-id="6864d-118">รับความเข้าใจข้อมูลที่สำคัญด้วย[DLP รายงาน](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="6864d-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="6864d-119">ดูรายละเอียดเฉพาะของเหตุการณ์ที่มีการ[รายงานเหตุการณ์](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="6864d-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
