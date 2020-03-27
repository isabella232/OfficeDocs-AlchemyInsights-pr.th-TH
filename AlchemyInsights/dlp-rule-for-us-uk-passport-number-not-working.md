---
title: กฎ DLP สําหรับหมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักรไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977125"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="24504-102">ปัญหาเกี่ยวกับ DLP -- US / UK หนังสือเดินทางหมายเลข</span><span class="sxs-lookup"><span data-stu-id="24504-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="24504-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="24504-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="24504-104">**ปัญหา DLP กับสหรัฐอเมริกา / สหราชอาณาจักรหมายเลขหนังสือเดินทาง**</span><span class="sxs-lookup"><span data-stu-id="24504-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="24504-105">คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขหนังสือเดินทางของสหรัฐอเมริกา / UK**เมื่อใช้ชนิดข้อมูลที่สําคัญ DLP ใน O365?</span><span class="sxs-lookup"><span data-stu-id="24504-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="24504-106">ถ้าเป็นเช่นนั้น, ให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นสําหรับสิ่งที่นโยบาย DLP กําลังมองหาเมื่อมีการประเมิน.</span><span class="sxs-lookup"><span data-stu-id="24504-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="24504-107">ตัวอย่างเช่น สําหรับนโยบาย**หมายเลขหนังสือเดินทางสหรัฐฯ/สหราชอาณาจักร**ที่กําหนดค่าด้วยระดับความเชื่อมั่น 75% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์</span><span class="sxs-lookup"><span data-stu-id="24504-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="24504-108">**[รูปแบบ: รูปแบบ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** ตัวเลข 9 หลัก</span><span class="sxs-lookup"><span data-stu-id="24504-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="24504-109">**[รูปแบบ: รูปแบบ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** เก้าหลักติดต่อกัน</span><span class="sxs-lookup"><span data-stu-id="24504-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="24504-110">**[เช็คซัม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** ไม่มีไม่มีเช็คซัม</span><span class="sxs-lookup"><span data-stu-id="24504-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="24504-111">**[ความหมาย:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** นโยบาย DLP มี 75% มั่นใจว่ามันตรวจพบชนิดของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:</span><span class="sxs-lookup"><span data-stu-id="24504-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="24504-112">ฟังก์ชันFunc_usa_uk_passportค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="24504-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="24504-113">พบคําสําคัญจากKeyword_passport</span><span class="sxs-lookup"><span data-stu-id="24504-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="24504-114">ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบาย**หมายเลขหนังสือเดินทางสหรัฐอเมริกา/สหราชอาณาจักร**: หมายเลขหนังสือเดินทางของสหรัฐอเมริกา 123456789</span><span class="sxs-lookup"><span data-stu-id="24504-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="24504-115">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จําเป็นสําหรับหมายเลข Passport ของสหรัฐอเมริกา/สหราชอาณาจักรที่จะตรวจพบสําหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[อะไรชนิดข้อมูลที่สําคัญค้นหาสําหรับ US/UK หมายเลขหนังสือเดินทาง](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="24504-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="24504-116">ใช้ชนิดข้อมูลที่ละเอียดอ่อนที่แตกต่างกัน[What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="24504-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  