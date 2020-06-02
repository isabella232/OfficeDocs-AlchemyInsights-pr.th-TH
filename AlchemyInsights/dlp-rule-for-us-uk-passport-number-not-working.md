---
title: กฎ DLP สําหรับสหรัฐอเมริกา / สหราชอาณาจักรหนังสือเดินทางหมายเลขไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507317"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="4eadf-102">ปัญหาเกี่ยวกับ DLP -- หมายเลขหนังสือเดินทางสหรัฐ / สหราชอาณาจักร</span><span class="sxs-lookup"><span data-stu-id="4eadf-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="4eadf-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้เรากําลังดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงมีอยู่มาก - โปรดเยี่ยมชม[SharePoint ออนไลน์ชั่วคราวการปรับปรุงคุณลักษณะ](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="4eadf-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4eadf-104">**ปัญหาเกี่ยวกับหมายเลขหนังสือเดินทางของสหรัฐฯ/สหราชอาณาจักร**</span><span class="sxs-lookup"><span data-stu-id="4eadf-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="4eadf-105">คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่มี**หมายเลขหนังสือเดินทางสหรัฐ / สหราชอาณาจักร**เมื่อใช้ประเภทข้อมูลที่สําคัญ DLP ใน O365?</span><span class="sxs-lookup"><span data-stu-id="4eadf-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="4eadf-106">ถ้าเป็นเช่นนั้น โปรดตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นสําหรับสิ่งที่นโยบาย DLP กําลังค้นหาเมื่อได้รับการประเมิน</span><span class="sxs-lookup"><span data-stu-id="4eadf-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="4eadf-107">ตัวอย่างเช่น สําหรับนโยบาย**หมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักร**ที่กําหนดค่าด้วยระดับความเชื่อมั่น 75% ต่อไปนี้จะถูกประเมินและต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์</span><span class="sxs-lookup"><span data-stu-id="4eadf-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="4eadf-108">**[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** เก้าหลัก</span><span class="sxs-lookup"><span data-stu-id="4eadf-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="4eadf-109">**[รูปแบบ: 10000](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** ตัวเลข 9 ตัวติดต่อกัน</span><span class="sxs-lookup"><span data-stu-id="4eadf-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="4eadf-110">**[เช็คซัม:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** ไม่มีไม่มีเช็คซัม</span><span class="sxs-lookup"><span data-stu-id="4eadf-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="4eadf-111">**[ความหมาย: 10000](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** นโยบาย DLP มีความมั่นใจ 75% ว่าตรวจพบประเภทของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:</span><span class="sxs-lookup"><span data-stu-id="4eadf-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4eadf-112">ฟังก์ชันFunc_usa_uk_passportค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="4eadf-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="4eadf-113">พบคําสําคัญจากKeyword_passport</span><span class="sxs-lookup"><span data-stu-id="4eadf-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="4eadf-114">ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบาย**หมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักร**: หมายเลขหนังสือเดินทางของสหรัฐอเมริกา 123456789</span><span class="sxs-lookup"><span data-stu-id="4eadf-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="4eadf-115">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จําเป็นสําหรับการตรวจพบหมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักรสําหรับเนื้อหาของคุณ ให้ดูในส่วนต่อไปนี้ในบทความนี้:[สิ่งที่ชนิดข้อมูลที่ละเอียดอ่อนมองหาหมายเลขหนังสือเดินทางสหรัฐอเมริกา /สหราชอาณาจักร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="4eadf-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="4eadf-116">การใช้ชนิดข้อมูลที่ละเอียดอ่อนในตัวชนิดอื่น ให้ดูบทความต่อไปนี้สําหรับข้อมูลเกี่ยวกับสิ่งที่จําเป็นสําหรับชนิดอื่น:[ชนิดข้อมูลที่สําคัญมีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="4eadf-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  