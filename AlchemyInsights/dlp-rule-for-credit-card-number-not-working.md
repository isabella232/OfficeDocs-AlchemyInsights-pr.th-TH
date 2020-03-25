---
title: กฎ DLP สําหรับหมายเลขบัตรเครดิตไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932462"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="eedcb-102">ปัญหา DLP กับหมายเลขบัตรเครดิต</span><span class="sxs-lookup"><span data-stu-id="eedcb-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="eedcb-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="eedcb-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="eedcb-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="eedcb-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="eedcb-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="eedcb-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="eedcb-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="eedcb-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="eedcb-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="eedcb-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="eedcb-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="eedcb-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="eedcb-109">**ปัญหา DLP กับหมายเลขบัตรเครดิต**</span><span class="sxs-lookup"><span data-stu-id="eedcb-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="eedcb-110">คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขบัตรเครดิต**เมื่อใช้ชนิดข้อมูลที่สําคัญ DLP ใน O365?</span><span class="sxs-lookup"><span data-stu-id="eedcb-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="eedcb-111">ถ้าเป็นเช่นนั้น โปรดตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นเพื่อทริกเกอร์นโยบาย DLP เมื่อมีประเมิน</span><span class="sxs-lookup"><span data-stu-id="eedcb-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="eedcb-112">ตัวอย่างเช่น สําหรับ**นโยบายบัตรเครดิต**ที่กําหนดค่าด้วยระดับความเชื่อมั่น 85% มีการประเมินต่อไปนี้ และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์:</span><span class="sxs-lookup"><span data-stu-id="eedcb-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="eedcb-113">**[รูปแบบ :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 หลักซึ่งสามารถจัดรูปแบบหรือไม่ได้จัดรูปแบบ (dddddddddddddddddddddd) และจะต้องผ่านการทดสอบ Luhn</span><span class="sxs-lookup"><span data-stu-id="eedcb-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="eedcb-114">**[รูปแบบ: รูปแบบ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** รูปแบบที่ซับซ้อนและแข็งแกร่งมากที่ตรวจจับการ์ดจากแบรนด์สําคัญๆ ทั่วโลก รวมถึง Visa, MasterCard, Discover Card, JCB, American Express, บัตรของขวัญ และบัตรอาหาร</span><span class="sxs-lookup"><span data-stu-id="eedcb-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="eedcb-115">**[เช็คซัม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** ใช่, การตรวจสอบ Luhn</span><span class="sxs-lookup"><span data-stu-id="eedcb-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="eedcb-116">**[ความหมาย:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** นโยบาย DLP คือ 85% มั่นใจว่ามันตรวจพบชนิดของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:</span><span class="sxs-lookup"><span data-stu-id="eedcb-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="eedcb-117">ฟังก์ชันFunc_credit_cardค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="eedcb-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="eedcb-118">หนึ่งต่อไปนี้เป็นจริง:</span><span class="sxs-lookup"><span data-stu-id="eedcb-118">One of the following is true:</span></span>

  - <span data-ttu-id="eedcb-119">พบคําสําคัญจากKeyword_cc_verification</span><span class="sxs-lookup"><span data-stu-id="eedcb-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="eedcb-120">พบคําหลักจากKeyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="eedcb-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="eedcb-121">ฟังก์ชันFunc_expiration_dateค้นหาวันที่ในรูปแบบวันที่ที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="eedcb-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="eedcb-122">เช็คซัมผ่าน</span><span class="sxs-lookup"><span data-stu-id="eedcb-122">The checksum passes</span></span>

    <span data-ttu-id="eedcb-123">ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบายหมายเลขบัตรเครดิต DLP:</span><span class="sxs-lookup"><span data-stu-id="eedcb-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="eedcb-124">วีซ่า: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="eedcb-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="eedcb-125">หมดอายุ: 2/2009</span><span class="sxs-lookup"><span data-stu-id="eedcb-125">Expires: 2/2009</span></span>

<span data-ttu-id="eedcb-126">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งจําเป็นสําหรับ**หมายเลขบัตรเครดิต**ที่จะตรวจพบสําหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[สิ่งที่ชนิดข้อมูลที่สําคัญที่มองหาบัตรเครดิต #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="eedcb-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="eedcb-127">ใช้ชนิดข้อมูลที่ละเอียดอ่อนที่แตกต่างกัน[What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="eedcb-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  