---
title: กฎ DLP สําหรับ SSN ไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507389"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="3aaeb-102">ปัญหาเกี่ยวกับหมายเลข DLP ประกันสังคม</span><span class="sxs-lookup"><span data-stu-id="3aaeb-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="3aaeb-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้เรากําลังดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงมีอยู่มาก - โปรดเยี่ยมชม[SharePoint ออนไลน์ชั่วคราวการปรับปรุงคุณลักษณะ](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="3aaeb-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="3aaeb-104">**ปัญหาเกี่ยวกับ SSNs DLP**</span><span class="sxs-lookup"><span data-stu-id="3aaeb-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="3aaeb-105">คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขประกันสังคม (SSN)** เมื่อใช้ชนิดข้อมูลที่สําคัญใน Microsoft 365 หรือไม่</span><span class="sxs-lookup"><span data-stu-id="3aaeb-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="3aaeb-106">หากเป็นเช่นนั้น โปรดตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นสําหรับนโยบาย DLP กําลังค้นหา</span><span class="sxs-lookup"><span data-stu-id="3aaeb-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="3aaeb-107">ตัวอย่างเช่น สําหรับนโยบาย SSN ที่กําหนดค่าด้วยระดับความเชื่อมั่น 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบสําหรับกฎเพื่อทริกเกอร์:</span><span class="sxs-lookup"><span data-stu-id="3aaeb-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="3aaeb-108">**[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 หลักซึ่งอาจอยู่ในรูปแบบการจัดรูปแบบหรือไม่จัดรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="3aaeb-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="3aaeb-109">**[รูปแบบ: 10000](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** สี่ฟังก์ชั่นมองหา SSNs ในรูปแบบที่แตกต่างกันสี่:</span><span class="sxs-lookup"><span data-stu-id="3aaeb-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="3aaeb-110">Func_ssnพบ SSNs ที่มีการจัดรูปแบบที่แข็งแกร่งก่อนปี 2011 ซึ่งจัดรูปแบบด้วยเครื่องหมายขีดกลางหรือช่องว่าง (ddd-ddd-ddd หรือ ddd ddd)</span><span class="sxs-lookup"><span data-stu-id="3aaeb-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="3aaeb-111">Func_unformatted_ssnพบ SSNs ที่มีการจัดรูปแบบที่แข็งแกร่งก่อน 2011 ที่ไม่มีการจัดรูปแบบเป็นตัวเลขต่อเนื่องเก้าหลัก (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="3aaeb-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="3aaeb-112">Func_randomized_formatted_ssnค้นหา SSNs post-2011 ที่มีการจัดรูปแบบด้วยเครื่องหมายขีดกลางหรือช่องว่าง (ddd-ddd-ddd หรือ ddd ddd)</span><span class="sxs-lookup"><span data-stu-id="3aaeb-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="3aaeb-113">Func_randomized_unformatted_ssnพบ SSNs โพสต์-2011 ที่ไม่ถูกจัดรูปแบบเป็นตัวเลขต่อเนื่องเก้าหลัก (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="3aaeb-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="3aaeb-114">**[เช็คซัม:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** ไม่มีไม่มีเช็คซัม</span><span class="sxs-lookup"><span data-stu-id="3aaeb-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="3aaeb-115">**[ความหมาย: 10000](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** นโยบาย DLP มีความมั่นใจ 85% ว่าตรวจพบประเภทของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:</span><span class="sxs-lookup"><span data-stu-id="3aaeb-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="3aaeb-116">[ฟังก์ชันFunc_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80)ค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="3aaeb-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="3aaeb-117">พบคําสําคัญจาก[Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="3aaeb-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="3aaeb-118">ตัวอย่างของคําหลักรวมถึง:*ประกันสังคม, ประกันสังคม # # , Soc Sec , SSN* .</span><span class="sxs-lookup"><span data-stu-id="3aaeb-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="3aaeb-119">ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบาย DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="3aaeb-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="3aaeb-120">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จําเป็นสําหรับ SSNs ที่จะตรวจพบสําหรับเนื้อหาของคุณ ให้ดูในส่วนต่อไปนี้ในบทความนี้:[ชนิดข้อมูลละเอียดอ่อนค้นหา SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="3aaeb-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="3aaeb-121">การใช้ชนิดข้อมูลที่ละเอียดอ่อนในตัวชนิดอื่น ให้ดูบทความต่อไปนี้สําหรับข้อมูลเกี่ยวกับสิ่งที่จําเป็นสําหรับชนิดอื่น:[ชนิดข้อมูลที่สําคัญมีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="3aaeb-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  