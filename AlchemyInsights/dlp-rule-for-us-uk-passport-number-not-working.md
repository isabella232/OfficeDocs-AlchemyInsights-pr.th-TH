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
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931281"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="a358c-102">ปัญหาเกี่ยวกับ DLP -- US / UK หนังสือเดินทางหมายเลข</span><span class="sxs-lookup"><span data-stu-id="a358c-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="a358c-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="a358c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a358c-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="a358c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a358c-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="a358c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a358c-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="a358c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a358c-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="a358c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a358c-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="a358c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a358c-109">**ปัญหา DLP กับสหรัฐอเมริกา / สหราชอาณาจักรหมายเลขหนังสือเดินทาง**</span><span class="sxs-lookup"><span data-stu-id="a358c-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="a358c-110">คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขหนังสือเดินทางของสหรัฐอเมริกา / UK**เมื่อใช้ชนิดข้อมูลที่สําคัญ DLP ใน O365?</span><span class="sxs-lookup"><span data-stu-id="a358c-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a358c-111">ถ้าเป็นเช่นนั้น, ให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นสําหรับสิ่งที่นโยบาย DLP กําลังมองหาเมื่อมีการประเมิน.</span><span class="sxs-lookup"><span data-stu-id="a358c-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="a358c-112">ตัวอย่างเช่น สําหรับนโยบาย**หมายเลขหนังสือเดินทางสหรัฐฯ/สหราชอาณาจักร**ที่กําหนดค่าด้วยระดับความเชื่อมั่น 75% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์</span><span class="sxs-lookup"><span data-stu-id="a358c-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="a358c-113">**[รูปแบบ: รูปแบบ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** ตัวเลข 9 หลัก</span><span class="sxs-lookup"><span data-stu-id="a358c-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="a358c-114">**[รูปแบบ: รูปแบบ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** เก้าหลักติดต่อกัน</span><span class="sxs-lookup"><span data-stu-id="a358c-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="a358c-115">**[เช็คซัม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** ไม่มีไม่มีเช็คซัม</span><span class="sxs-lookup"><span data-stu-id="a358c-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="a358c-116">**[ความหมาย:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** นโยบาย DLP มี 75% มั่นใจว่ามันตรวจพบชนิดของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:</span><span class="sxs-lookup"><span data-stu-id="a358c-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a358c-117">ฟังก์ชันFunc_usa_uk_passportค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="a358c-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="a358c-118">พบคําสําคัญจากKeyword_passport</span><span class="sxs-lookup"><span data-stu-id="a358c-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="a358c-119">ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบาย**หมายเลขหนังสือเดินทางสหรัฐอเมริกา/สหราชอาณาจักร**: หมายเลขหนังสือเดินทางของสหรัฐอเมริกา 123456789</span><span class="sxs-lookup"><span data-stu-id="a358c-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="a358c-120">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จําเป็นสําหรับหมายเลข Passport ของสหรัฐอเมริกา/สหราชอาณาจักรที่จะตรวจพบสําหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[อะไรชนิดข้อมูลที่สําคัญค้นหาสําหรับ US/UK หมายเลขหนังสือเดินทาง](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="a358c-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="a358c-121">ใช้ชนิดข้อมูลที่ละเอียดอ่อนที่แตกต่างกัน[What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a358c-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  