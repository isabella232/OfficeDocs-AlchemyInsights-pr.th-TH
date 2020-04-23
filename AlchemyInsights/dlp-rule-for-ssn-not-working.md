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
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788721"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="77ad1-102">ปัญหา DLP กับหมายเลขประกันสังคม</span><span class="sxs-lookup"><span data-stu-id="77ad1-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="77ad1-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="77ad1-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="77ad1-104">**ปัญหา DLP กับ SSNs**</span><span class="sxs-lookup"><span data-stu-id="77ad1-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="77ad1-105">คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขประกันสังคม (SSN)** เมื่อใช้ชนิดข้อมูลที่สําคัญใน Microsoft 365 หรือไม่</span><span class="sxs-lookup"><span data-stu-id="77ad1-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="77ad1-106">ถ้าเป็นเช่นนั้น, ให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นสําหรับสิ่งที่นโยบาย DLP กําลังมองหา.</span><span class="sxs-lookup"><span data-stu-id="77ad1-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="77ad1-107">ตัวอย่างเช่น สําหรับนโยบาย SSN ที่กําหนดค่าด้วยระดับความเชื่อมั่น 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์:</span><span class="sxs-lookup"><span data-stu-id="77ad1-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="77ad1-108">**[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 หลัก ซึ่งอาจจะเป็นรูปแบบที่จัดรูปแบบหรือรูปแบบไม่ได้จัดรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="77ad1-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="77ad1-109">**[รูปแบบ: รูปแบบ](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** สี่ฟังก์ชั่นมองหา SSNs ในสี่รูปแบบที่แตกต่างกัน:</span><span class="sxs-lookup"><span data-stu-id="77ad1-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="77ad1-110">Func_ssnค้นหา SSN ที่มีการจัดรูปแบบที่แข็งแกร่งก่อน 2011 ที่มีการจัดรูปแบบด้วยเครื่องหมายขีดคั่นหรือช่องว่าง (ddd-dddd หรือ ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="77ad1-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="77ad1-111">Func_unformatted_ssnค้นหา SSN ที่มีการจัดรูปแบบที่แข็งแกร่งก่อน 2011 ซึ่งยังไม่ได้จัดรูปแบบเป็นตัวเลขต่อเนื่องเก้าหลัก (dddddddddd)</span><span class="sxs-lookup"><span data-stu-id="77ad1-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="77ad1-112">Func_randomized_formatted_ssnพบ SSN หลัง 2011 ที่ถูกจัดรูปแบบด้วยเครื่องหมายขีดคั่นหรือช่องว่าง (ddd-dddd หรือ ddd ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="77ad1-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="77ad1-113">Func_randomized_unformatted_ssnพบ SSN หลัง 2011 ที่ยังไม่ฟอร์แมตเป็นตัวเลขติดต่อกันเก้าหลัก (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="77ad1-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="77ad1-114">**[เช็คซัม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** ไม่มีไม่มีเช็คซัม</span><span class="sxs-lookup"><span data-stu-id="77ad1-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="77ad1-115">**[ความหมาย:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** นโยบาย DLP คือ 85% มั่นใจว่ามันตรวจพบชนิดของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:</span><span class="sxs-lookup"><span data-stu-id="77ad1-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="77ad1-116">[ฟังก์ชันFunc_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)ค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="77ad1-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="77ad1-117">พบคําสําคัญจาก[Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="77ad1-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="77ad1-118">ตัวอย่างของคําสําคัญได้แก่:*ประกันสังคม, ประกันสังคม# Soc Sec, SSN*</span><span class="sxs-lookup"><span data-stu-id="77ad1-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="77ad1-119">ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบาย DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="77ad1-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="77ad1-120">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จําเป็นสําหรับ SSNs จะถูกตรวจพบสําหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[อะไรชนิดข้อมูลที่สําคัญที่มองหา SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="77ad1-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="77ad1-121">ใช้ชนิดข้อมูลที่ละเอียดอ่อนที่แตกต่างกัน[What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="77ad1-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  