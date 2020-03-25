---
title: กฎ DLP สําหรับหมายเลขบัญชีธนาคารของสหรัฐอเมริกาไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932569"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="96e42-102">ปัญหา DLP กับหมายเลขบัญชีธนาคารของสหรัฐอเมริกา</span><span class="sxs-lookup"><span data-stu-id="96e42-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="96e42-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="96e42-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="96e42-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="96e42-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="96e42-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="96e42-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="96e42-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="96e42-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="96e42-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="96e42-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="96e42-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="96e42-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="96e42-109">**ปัญหา DLP กับหมายเลขบัญชีธนาคารของสหรัฐอเมริกา**</span><span class="sxs-lookup"><span data-stu-id="96e42-109">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="96e42-110">คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่ประกอบด้วย**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**เมื่อใช้ชนิดข้อมูลที่สําคัญ DLP ใน O365 หรือไม่</span><span class="sxs-lookup"><span data-stu-id="96e42-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="96e42-111">ถ้าเป็นเช่นนั้น, ให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นสําหรับสิ่งที่นโยบาย DLP กําลังมองหาเมื่อมีการประเมิน.</span><span class="sxs-lookup"><span data-stu-id="96e42-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="96e42-112">ตัวอย่างเช่น สําหรับนโยบาย**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**ที่กําหนดค่าด้วยระดับความเชื่อมั่น 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์:</span><span class="sxs-lookup"><span data-stu-id="96e42-112">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="96e42-113">**[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8- 17หลัก</span><span class="sxs-lookup"><span data-stu-id="96e42-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="96e42-114">**[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8- 17หลักติดต่อกันของ</span><span class="sxs-lookup"><span data-stu-id="96e42-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="96e42-115">**[เช็คซัม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** ไม่มีไม่มีเช็คซัม</span><span class="sxs-lookup"><span data-stu-id="96e42-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="96e42-116">**[ความหมาย:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** นโยบาย DLP มี 75% มั่นใจว่ามันตรวจพบชนิดของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:</span><span class="sxs-lookup"><span data-stu-id="96e42-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="96e42-117">นิพจน์ทั่วไปRegex_usa_bank_account_numberพบเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="96e42-117">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="96e42-118">พบคําสําคัญจากKeyword_usa_Bank_Account</span><span class="sxs-lookup"><span data-stu-id="96e42-118">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="96e42-119">ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบาย**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**: การตรวจสอบบัญชี 78344011</span><span class="sxs-lookup"><span data-stu-id="96e42-119">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="96e42-120">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งจําเป็นสําหรับ**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**ที่จะตรวจพบสําหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[อะไรชนิดข้อมูลที่สําคัญค้นหาหมายเลขบัญชีธนาคารของสหรัฐอเมริกา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="96e42-120">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="96e42-121">ใช้ชนิดข้อมูลที่ละเอียดอ่อนที่แตกต่างกัน[What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="96e42-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  