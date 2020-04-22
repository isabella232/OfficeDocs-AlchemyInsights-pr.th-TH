---
title: กฎ DLP สําหรับหมายเลขบัญชีธนาคารของสหรัฐอเมริกาไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 45aa50f6c3505468e902e58faf698205f93f9264
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704058"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="1b1a0-102">ปัญหา DLP กับหมายเลขบัญชีธนาคารของสหรัฐอเมริกา</span><span class="sxs-lookup"><span data-stu-id="1b1a0-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="1b1a0-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="1b1a0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="1b1a0-104">**ปัญหา DLP กับหมายเลขบัญชีธนาคารของสหรัฐอเมริกา**</span><span class="sxs-lookup"><span data-stu-id="1b1a0-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="1b1a0-105">คุณมีปัญหากับ**การป้องกันข้อมูลสูญหาย (DLP)** ไม่ทํางานสําหรับเนื้อหาที่ประกอบด้วย**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**เมื่อใช้ชนิดข้อมูลที่สําคัญ DLP ใน O365 หรือไม่</span><span class="sxs-lookup"><span data-stu-id="1b1a0-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="1b1a0-106">ถ้าเป็นเช่นนั้น, ให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จําเป็นสําหรับสิ่งที่นโยบาย DLP กําลังมองหาเมื่อมีการประเมิน.</span><span class="sxs-lookup"><span data-stu-id="1b1a0-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="1b1a0-107">ตัวอย่างเช่น สําหรับนโยบาย**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**ที่กําหนดค่าด้วยระดับความเชื่อมั่น 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบสําหรับกฎที่จะทริกเกอร์:</span><span class="sxs-lookup"><span data-stu-id="1b1a0-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="1b1a0-108">**[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8- 17หลัก</span><span class="sxs-lookup"><span data-stu-id="1b1a0-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="1b1a0-109">**[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8- 17หลักติดต่อกันของ</span><span class="sxs-lookup"><span data-stu-id="1b1a0-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="1b1a0-110">**[เช็คซัม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** ไม่มีไม่มีเช็คซัม</span><span class="sxs-lookup"><span data-stu-id="1b1a0-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="1b1a0-111">**[ความหมาย:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** นโยบาย DLP มี 75% มั่นใจว่ามันตรวจพบชนิดของข้อมูลที่ละเอียดอ่อนนี้ถ้าภายในความใกล้ชิดของ 300 ตัวอักษร:</span><span class="sxs-lookup"><span data-stu-id="1b1a0-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="1b1a0-112">นิพจน์ทั่วไปRegex_usa_bank_account_numberพบเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="1b1a0-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="1b1a0-113">พบคําสําคัญจากKeyword_usa_Bank_Account</span><span class="sxs-lookup"><span data-stu-id="1b1a0-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="1b1a0-114">ตัวอย่างต่อไปนี้จะทริกเกอร์สําหรับนโยบาย**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**: การตรวจสอบบัญชี 78344011</span><span class="sxs-lookup"><span data-stu-id="1b1a0-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="1b1a0-115">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งจําเป็นสําหรับ**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**ที่จะตรวจพบสําหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[อะไรชนิดข้อมูลที่สําคัญค้นหาหมายเลขบัญชีธนาคารของสหรัฐอเมริกา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="1b1a0-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="1b1a0-116">ใช้ชนิดข้อมูลที่ละเอียดอ่อนที่แตกต่างกัน[What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="1b1a0-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  