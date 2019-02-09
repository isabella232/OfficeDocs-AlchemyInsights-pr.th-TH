---
title: กฎ DLP สำหรับสหรัฐอเมริกา / หมาย เลขหนังสือเดินทางสหราชอาณาจักรที่ไม่ทำงาน
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: ec7f11676982b56a46c83bf276c2212ce765ba6f
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786717"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="04351-102">ปัญหาเกี่ยวกับ DLP - สหรัฐอเมริกา / หมายเลขหนังสือเดินทางสหราชอาณาจักร</span><span class="sxs-lookup"><span data-stu-id="04351-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="04351-p101">คุณกำลังมีปัญหากับ**การป้องกันการสูญเสียข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่ประกอบด้วยการ**ของสหรัฐอเมริกา / หมายเลขหนังสือเดินทางสหราชอาณาจักร**เมื่อใช้ชนิดข้อมูลที่เป็นความลับ DLP ใน O365 หรือไม่ ถ้าเป็นเช่นนั้น ทำให้แน่ใจว่าเนื้อหาของคุณประกอบด้วยข้อมูลที่จำเป็นสำหรับสิ่งนโยบาย DLP จะค้นหาเมื่อถูกประเมิน</span><span class="sxs-lookup"><span data-stu-id="04351-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="04351-105">ตัวอย่างเช่น สำหรับการ**ของสหรัฐอเมริกา / หมายเลขหนังสือเดินทางสหราชอาณาจักร**นโยบายการตั้งค่าคอนฟิก ด้วยระดับความเชื่อมั่น 75% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบกฎเพื่อทริกเกอร์</span><span class="sxs-lookup"><span data-stu-id="04351-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="04351-106">**[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** ตัวเลขเก้าหลัก</span><span class="sxs-lookup"><span data-stu-id="04351-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="04351-107">**[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** ตัวเลขที่ต่อเนื่องกันเก้า</span><span class="sxs-lookup"><span data-stu-id="04351-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="04351-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** ไม่มี ไม่มี Checksum ไม่มี</span><span class="sxs-lookup"><span data-stu-id="04351-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="04351-109">**[คำนิยาม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** นโยบาย DLP คือ 75% มั่นใจจะได้ตรวจพบชนิดข้อมูลที่เป็นความลับนี้ if ภายในมีความใกล้เคียง 300 อักขระ:</span><span class="sxs-lookup"><span data-stu-id="04351-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="04351-110">ฟังก์ชัน Func_usa_uk_passport ค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="04351-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="04351-111">พบคำสำคัญจาก Keyword_passport</span><span class="sxs-lookup"><span data-stu-id="04351-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="04351-112">ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับการ**ของสหรัฐอเมริกา / หมายเลขหนังสือเดินทางสหราชอาณาจักร**นโยบาย: หมายเลขหนังสือเดินทางของสหรัฐอเมริกา 123456789</span><span class="sxs-lookup"><span data-stu-id="04351-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="04351-113">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จำเป็นสำหรับประเทศ / หมายเลขหนังสือเดินทางสหราชอาณาจักรสามารถตรวจพบคอมพิวเตอร์สำหรับเนื้อหาของคุณ ดูหัวข้อต่อไปนี้ในบทความนี้:[มองหาสิ่งเป็นความลับชนิดข้อมูลสำหรับสหรัฐอเมริกา / หมายเลขหนังสือเดินทางสหราชอาณาจักร](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="04351-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="04351-114">โดยใช้ชนิดข้อมูลที่สำคัญในตัวแตกต่างกัน ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งจำเป็นสำหรับชนิดอื่น ๆ:[สิ่งสำคัญชนิดข้อมูลค้นหา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="04351-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

