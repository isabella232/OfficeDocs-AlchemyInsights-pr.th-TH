---
title: กฎ DLP สำหรับ SSN ไม่ทำงาน
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679388"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="f4927-102">ปัญหา DLP เกี่ยวกับหมายเลขประกันสังคม</span><span class="sxs-lookup"><span data-stu-id="f4927-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="f4927-103">**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="f4927-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="f4927-104">**ปัญหา DLP เกี่ยวกับ SSNs**</span><span class="sxs-lookup"><span data-stu-id="f4927-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="f4927-105">คุณมีปัญหาเกี่ยวกับการ **ป้องกันการสูญหายของข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่มี **หมายเลขประกันสังคม (SSN)** เมื่อใช้ชนิดข้อมูลที่เป็นความลับใน Microsoft ๓๖๕ใช่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="f4927-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="f4927-106">ถ้าเป็นเช่นนั้นตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จำเป็นสำหรับนโยบาย DLP ที่กำลังค้นหา</span><span class="sxs-lookup"><span data-stu-id="f4927-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="f4927-107">ตัวอย่างเช่นสำหรับนโยบาย SSN ที่กำหนดค่าด้วยระดับความเชื่อมั่นของ๘๕% ดังต่อไปนี้จะถูกประเมินและต้องถูกตรวจพบสำหรับกฎที่จะทริกเกอร์:</span><span class="sxs-lookup"><span data-stu-id="f4927-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="f4927-108">**[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 หลักซึ่งอาจอยู่ในรูปแบบที่จัดรูปแบบหรือรูปแบบที่ไม่มีการจัดรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="f4927-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="f4927-109">**[ลวดลาย:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** ฟังก์ชันสี่ฟังก์ชันสำหรับ SSNs ในรูปแบบที่แตกต่างกันสี่รูปแบบดังนี้</span><span class="sxs-lookup"><span data-stu-id="f4927-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="f4927-110">Func_ssn ค้นหา SSNs ด้วยการจัดรูปแบบที่มีความแข็งแกร่งล่วงหน้า๒๐๑๑ที่จัดรูปแบบด้วยเส้นประหรือช่องว่าง (ddd-ดี dddd หรือ ddd พิ่ม dddd)</span><span class="sxs-lookup"><span data-stu-id="f4927-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="f4927-111">Func_unformatted_ssn ค้นหา SSNs ด้วยการจัดรูปแบบที่มีความแข็งแกร่งล่วงหน้า๒๐๑๑ที่ได้รับการจัดรูปแบบเป็นตัวเลขติดกัน9ตัว (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="f4927-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="f4927-112">Func_randomized_formatted_ssn ค้นหา SSNs post-๒๐๑๑ที่จัดรูปแบบด้วยเส้นประหรือช่องว่าง (ddd-ดี-dddd หรือ ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="f4927-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="f4927-113">Func_randomized_unformatted_ssn ค้นหา SSNs post-๒๐๑๑ที่ได้รับการจัดรูปแบบเป็นตัวเลขที่ติดต่อกันได้9ตัว (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="f4927-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="f4927-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** ไม่มี Checksum</span><span class="sxs-lookup"><span data-stu-id="f4927-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="f4927-115">**[ข้อกำหนด:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** นโยบาย DLP มีความมั่นใจ๘๕% ว่าจะตรวจพบข้อมูลที่เป็นความลับชนิดนี้ในกรณีที่มีอักขระ๓๐๐ที่อยู่ในความใกล้เคียง:</span><span class="sxs-lookup"><span data-stu-id="f4927-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="f4927-116">[ฟังก์ชัน Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80)ค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="f4927-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="f4927-117">พบคำสำคัญจาก[Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="f4927-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="f4927-118">ตัวอย่างของคำสำคัญประกอบด้วย: การ*รักษาความปลอดภัยทางสังคม, ความมั่นคงทางสังคม #, Soc Sec, SSN*</span><span class="sxs-lookup"><span data-stu-id="f4927-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="f4927-119">ตัวอย่างเช่นตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับนโยบาย DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="f4927-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="f4927-120">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จำเป็นสำหรับการตรวจพบ SSNs สำหรับเนื้อหาของคุณให้ดูส่วนต่อไปนี้ในบทความนี้: [ชนิดข้อมูลที่เป็นความลับที่มีลักษณะสำหรับ SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="f4927-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="f4927-121">การใช้ชนิดข้อมูลที่มีความสำคัญที่มีอยู่แล้วภายในที่แตกต่างกันให้ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งที่จำเป็นสำหรับชนิดอื่นๆ: [ชนิดข้อมูลที่เป็นความลับที่มีลักษณะสำหรับ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="f4927-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  