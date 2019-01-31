---
title: กฎ DLP สำหรับ SSN ไม่ทำงาน
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 7242bf2b101b45fec0fe00ab33fa6db150004ee5
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657378"
---
<span data-ttu-id="175dc-p101">คุณกำลังมีปัญหากับ**การป้องกันการสูญเสียข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่ประกอบด้วยตัว**เลขประกันสังคม (SSN)** เมื่อใช้ชนิดข้อมูลที่เป็นความลับใน Office 365 ได้อย่างไร ถ้าเป็นเช่นนั้น ทำให้แน่ใจว่า เนื้อหาของคุณประกอบด้วยข้อมูลที่จำเป็นสำหรับสิ่งที่นโยบาย DLP ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="175dc-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365? If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="175dc-104">ตัวอย่างเช่น สำหรับ SSN มีนโยบายการกำหนดค่า ด้วยระดับความเชื่อมั่นของ 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบกฎเพื่อทริกเกอร์:</span><span class="sxs-lookup"><span data-stu-id="175dc-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="175dc-105">**[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** ตัวเลข 9 หลัก ซึ่งอาจจะอยู่ในรูปแบบการจัดรูปแบบ หรือไม่จัดรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="175dc-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="175dc-106">**[รูปแบบ:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** สี่ฟังก์ชันที่ค้นหา SSNs ในสี่รูปแบบที่แตกต่างกัน:</span><span class="sxs-lookup"><span data-stu-id="175dc-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="175dc-107">Func_ssn ค้นหา SSNs กับ 2011 ก่อนที่คาดเดายากจัดรูปแบบที่ถูกจัดรูปแบบ ด้วยเส้นประหรือช่องว่าง (ววววววววว OR ววววววววว)</span><span class="sxs-lookup"><span data-stu-id="175dc-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="175dc-108">Func_unformatted_ssn ค้นหา SSNs กับ 2011 ก่อนที่คาดเดายากจัดรูปแบบที่ไม่จัดรูปแบบเป็นตัวเลขติดกันเก้า (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="175dc-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="175dc-109">Func_randomized_formatted_ssn ค้นหา SSNs 2011 ลงรายการบัญชีที่มีการจัดรูปแบบ ด้วยเส้นประหรือช่องว่าง (ววววววววว OR ววววววววว)</span><span class="sxs-lookup"><span data-stu-id="175dc-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="175dc-110">Func_randomized_unformatted_ssn ค้นหา SSNs 2011 ลงรายการบัญชีที่จะไม่จัดรูปแบบเป็นตัวเลขติดกันเก้า (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="175dc-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="175dc-111">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** ไม่มี ไม่มี Checksum ไม่มี</span><span class="sxs-lookup"><span data-stu-id="175dc-111">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="175dc-112">**[คำนิยาม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** นโยบาย DLP คือ 85% มั่นใจจะได้ตรวจพบชนิดข้อมูลที่เป็นความลับนี้ if ภายในมีความใกล้เคียง 300 อักขระ:</span><span class="sxs-lookup"><span data-stu-id="175dc-112">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="175dc-113">[ฟังก์ชัน Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)ค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="175dc-113">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="175dc-p102">พบคำสำคัญจาก[Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) มีตัวอย่างของคำสำคัญ:*สังคม สังคม Soc วินาที SSN* ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับนโยบาย DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="175dc-p102">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found. Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  . For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="175dc-117">หากต้องการข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จำเป็นสำหรับ SSNs สามารถตรวจพบคอมพิวเตอร์สำหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[สิ่งสำคัญชนิดข้อมูลค้นหา SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="175dc-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="175dc-118">โดยใช้ชนิดข้อมูลที่สำคัญในตัวแตกต่างกัน ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งจำเป็นสำหรับชนิดอื่น ๆ:[สิ่งสำคัญชนิดข้อมูลค้นหา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="175dc-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

