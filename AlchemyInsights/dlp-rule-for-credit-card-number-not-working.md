---
title: กฎ DLP สําหรับหมายเลขบัตรเครดิตไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507425"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="8641d-102">ปัญหาเกี่ยวกับหมายเลขบัตรเครดิต DLP</span><span class="sxs-lookup"><span data-stu-id="8641d-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="8641d-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้เรากําลังดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงมีอยู่มาก - โปรดเยี่ยมชม[SharePoint ออนไลน์ชั่วคราวการปรับปรุงคุณลักษณะ](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="8641d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="8641d-104">**ปัญหาเกี่ยวกับหมายเลขบัตรเครดิต DLP**</span><span class="sxs-lookup"><span data-stu-id="8641d-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="8641d-105">คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขบัตรเครดิต**เมื่อใช้ประเภทข้อมูลที่สําคัญ DLP ใน O365?</span><span class="sxs-lookup"><span data-stu-id="8641d-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="8641d-106">ถ้าเป็นเช่นนั้น โปรดตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นในการเรียกใช้นโยบาย DLP เมื่อได้รับการประเมิน</span><span class="sxs-lookup"><span data-stu-id="8641d-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="8641d-107">ตัวอย่างเช่น สําหรับ**นโยบายบัตรเครดิต**ที่กําหนดค่าด้วยระดับความเชื่อมั่น 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์:</span><span class="sxs-lookup"><span data-stu-id="8641d-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="8641d-108">**[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 หลักที่สามารถจัดรูปแบบหรือไม่ได้จัดรูปแบบ (ddddddddddddd) และต้องผ่านการทดสอบ Luhn</span><span class="sxs-lookup"><span data-stu-id="8641d-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="8641d-109">**[รูปแบบ: 10000](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** รูปแบบที่ซับซ้อนมากและแข็งแกร่งที่ตรวจพบบัตรจากแบรนด์สําคัญทั้งหมดทั่วโลกรวมทั้งวีซ่ามาสเตอร์การ์ดการ์ดค้นพบ JCB อเมริกันเอ็กซ์เพรสบัตรของขวัญและบัตรร้านอาหาร</span><span class="sxs-lookup"><span data-stu-id="8641d-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="8641d-110">**[เช็คซัม:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** ใช่ เช็คซัมลูน</span><span class="sxs-lookup"><span data-stu-id="8641d-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="8641d-111">**[ความหมาย: 10000](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** นโยบาย DLP มีความมั่นใจ 85% ว่าตรวจพบประเภทของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:</span><span class="sxs-lookup"><span data-stu-id="8641d-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="8641d-112">ฟังก์ชันFunc_credit_cardค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="8641d-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="8641d-113">หนึ่งในต่อไปนี้เป็นจริง:</span><span class="sxs-lookup"><span data-stu-id="8641d-113">One of the following is true:</span></span>

  - <span data-ttu-id="8641d-114">พบคําสําคัญจากKeyword_cc_verification</span><span class="sxs-lookup"><span data-stu-id="8641d-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="8641d-115">พบคําสําคัญจาก Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="8641d-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="8641d-116">ฟังก์ชันFunc_expiration_dateค้นหาวันที่ในรูปแบบวันที่ที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="8641d-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="8641d-117">เช็คซัมผ่าน</span><span class="sxs-lookup"><span data-stu-id="8641d-117">The checksum passes</span></span>

    <span data-ttu-id="8641d-118">ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบายหมายเลขบัตรเครดิต DLP:</span><span class="sxs-lookup"><span data-stu-id="8641d-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="8641d-119">วีซ่า: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="8641d-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="8641d-120">หมดอายุ: 2/2009</span><span class="sxs-lookup"><span data-stu-id="8641d-120">Expires: 2/2009</span></span>

<span data-ttu-id="8641d-121">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จําเป็นสําหรับ**การตรวจพบหมายเลขบัตรเครดิต**สําหรับเนื้อหาของคุณ โปรดดูส่วนต่อไปนี้ในบทความนี้:[สิ่งที่ประเภทข้อมูลที่สําคัญมองหาบัตรเครดิต#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="8641d-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="8641d-122">การใช้ชนิดข้อมูลที่ละเอียดอ่อนในตัวชนิดอื่น ให้ดูบทความต่อไปนี้สําหรับข้อมูลเกี่ยวกับสิ่งที่จําเป็นสําหรับชนิดอื่น:[ชนิดข้อมูลที่สําคัญมีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="8641d-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  