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
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977217"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="d4e6b-102">ปัญหา DLP กับหมายเลขบัตรเครดิต</span><span class="sxs-lookup"><span data-stu-id="d4e6b-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="d4e6b-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="d4e6b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d4e6b-104">**ปัญหา DLP กับหมายเลขบัตรเครดิต**</span><span class="sxs-lookup"><span data-stu-id="d4e6b-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="d4e6b-105">คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขบัตรเครดิต**เมื่อใช้ชนิดข้อมูลที่สําคัญ DLP ใน O365?</span><span class="sxs-lookup"><span data-stu-id="d4e6b-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d4e6b-106">ถ้าเป็นเช่นนั้น โปรดตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นเพื่อทริกเกอร์นโยบาย DLP เมื่อมีประเมิน</span><span class="sxs-lookup"><span data-stu-id="d4e6b-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="d4e6b-107">ตัวอย่างเช่น สําหรับ**นโยบายบัตรเครดิต**ที่กําหนดค่าด้วยระดับความเชื่อมั่น 85% มีการประเมินต่อไปนี้ และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์:</span><span class="sxs-lookup"><span data-stu-id="d4e6b-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d4e6b-108">**[รูปแบบ :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 หลักซึ่งสามารถจัดรูปแบบหรือไม่ได้จัดรูปแบบ (dddddddddddddddddddddd) และจะต้องผ่านการทดสอบ Luhn</span><span class="sxs-lookup"><span data-stu-id="d4e6b-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="d4e6b-109">**[รูปแบบ: รูปแบบ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** รูปแบบที่ซับซ้อนและแข็งแกร่งมากที่ตรวจจับการ์ดจากแบรนด์สําคัญๆ ทั่วโลก รวมถึง Visa, MasterCard, Discover Card, JCB, American Express, บัตรของขวัญ และบัตรอาหาร</span><span class="sxs-lookup"><span data-stu-id="d4e6b-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="d4e6b-110">**[เช็คซัม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** ใช่, การตรวจสอบ Luhn</span><span class="sxs-lookup"><span data-stu-id="d4e6b-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="d4e6b-111">**[ความหมาย:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** นโยบาย DLP คือ 85% มั่นใจว่ามันตรวจพบชนิดของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:</span><span class="sxs-lookup"><span data-stu-id="d4e6b-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d4e6b-112">ฟังก์ชันFunc_credit_cardค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="d4e6b-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d4e6b-113">หนึ่งต่อไปนี้เป็นจริง:</span><span class="sxs-lookup"><span data-stu-id="d4e6b-113">One of the following is true:</span></span>

  - <span data-ttu-id="d4e6b-114">พบคําสําคัญจากKeyword_cc_verification</span><span class="sxs-lookup"><span data-stu-id="d4e6b-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="d4e6b-115">พบคําหลักจากKeyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="d4e6b-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="d4e6b-116">ฟังก์ชันFunc_expiration_dateค้นหาวันที่ในรูปแบบวันที่ที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="d4e6b-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="d4e6b-117">เช็คซัมผ่าน</span><span class="sxs-lookup"><span data-stu-id="d4e6b-117">The checksum passes</span></span>

    <span data-ttu-id="d4e6b-118">ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบายหมายเลขบัตรเครดิต DLP:</span><span class="sxs-lookup"><span data-stu-id="d4e6b-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="d4e6b-119">วีซ่า: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="d4e6b-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="d4e6b-120">หมดอายุ: 2/2009</span><span class="sxs-lookup"><span data-stu-id="d4e6b-120">Expires: 2/2009</span></span>

<span data-ttu-id="d4e6b-121">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งจําเป็นสําหรับ**หมายเลขบัตรเครดิต**ที่จะตรวจพบสําหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[สิ่งที่ชนิดข้อมูลที่สําคัญที่มองหาบัตรเครดิต #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="d4e6b-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="d4e6b-122">ใช้ชนิดข้อมูลที่ละเอียดอ่อนที่แตกต่างกัน[What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d4e6b-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  