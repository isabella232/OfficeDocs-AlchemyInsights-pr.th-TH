---
title: กฎ DLP สําหรับ SSN ไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932555"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="42ac6-102">ปัญหา DLP กับหมายเลขประกันสังคม</span><span class="sxs-lookup"><span data-stu-id="42ac6-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="42ac6-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="42ac6-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="42ac6-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="42ac6-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="42ac6-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="42ac6-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="42ac6-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="42ac6-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="42ac6-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="42ac6-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="42ac6-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="42ac6-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="42ac6-109">**ปัญหา DLP กับ SSNs**</span><span class="sxs-lookup"><span data-stu-id="42ac6-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="42ac6-110">คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขประกันสังคม (SSN)** เมื่อใช้ชนิดข้อมูลที่สําคัญใน Office 365 หรือไม่</span><span class="sxs-lookup"><span data-stu-id="42ac6-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="42ac6-111">ถ้าเป็นเช่นนั้น, ให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นสําหรับสิ่งที่นโยบาย DLP กําลังมองหา.</span><span class="sxs-lookup"><span data-stu-id="42ac6-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="42ac6-112">ตัวอย่างเช่น สําหรับนโยบาย SSN ที่กําหนดค่าด้วยระดับความเชื่อมั่น 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์:</span><span class="sxs-lookup"><span data-stu-id="42ac6-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="42ac6-113">**[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 หลัก ซึ่งอาจจะเป็นรูปแบบที่จัดรูปแบบหรือรูปแบบไม่ได้จัดรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="42ac6-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="42ac6-114">**[รูปแบบ: รูปแบบ](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** สี่ฟังก์ชั่นมองหา SSNs ในสี่รูปแบบที่แตกต่างกัน:</span><span class="sxs-lookup"><span data-stu-id="42ac6-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="42ac6-115">Func_ssnค้นหา SSN ที่มีการจัดรูปแบบที่แข็งแกร่งก่อน 2011 ที่มีการจัดรูปแบบด้วยเครื่องหมายขีดคั่นหรือช่องว่าง (ddd-dddd หรือ ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="42ac6-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="42ac6-116">Func_unformatted_ssnค้นหา SSN ที่มีการจัดรูปแบบที่แข็งแกร่งก่อน 2011 ซึ่งยังไม่ได้จัดรูปแบบเป็นตัวเลขต่อเนื่องเก้าหลัก (dddddddddd)</span><span class="sxs-lookup"><span data-stu-id="42ac6-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="42ac6-117">Func_randomized_formatted_ssnพบ SSN หลัง 2011 ที่ถูกจัดรูปแบบด้วยเครื่องหมายขีดคั่นหรือช่องว่าง (ddd-dddd หรือ ddd ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="42ac6-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="42ac6-118">Func_randomized_unformatted_ssnพบ SSN หลัง 2011 ที่ยังไม่ฟอร์แมตเป็นตัวเลขติดต่อกันเก้าหลัก (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="42ac6-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="42ac6-119">**[เช็คซัม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** ไม่มีไม่มีเช็คซัม</span><span class="sxs-lookup"><span data-stu-id="42ac6-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="42ac6-120">**[ความหมาย:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** นโยบาย DLP คือ 85% มั่นใจว่ามันตรวจพบชนิดของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:</span><span class="sxs-lookup"><span data-stu-id="42ac6-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="42ac6-121">[ฟังก์ชันFunc_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)ค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="42ac6-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="42ac6-122">พบคําสําคัญจาก[Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="42ac6-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="42ac6-123">ตัวอย่างของคําสําคัญได้แก่:*ประกันสังคม, ประกันสังคม# Soc Sec, SSN*</span><span class="sxs-lookup"><span data-stu-id="42ac6-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="42ac6-124">ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบาย DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="42ac6-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="42ac6-125">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จําเป็นสําหรับ SSNs จะถูกตรวจพบสําหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[อะไรชนิดข้อมูลที่สําคัญที่มองหา SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="42ac6-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="42ac6-126">ใช้ชนิดข้อมูลที่ละเอียดอ่อนที่แตกต่างกัน[What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="42ac6-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  