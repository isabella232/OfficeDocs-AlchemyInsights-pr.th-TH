---
title: กฎ DLP สำหรับหมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักรไม่ทำงาน
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679243"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="11cc9-102">ปัญหาเกี่ยวกับ DLP-หมายเลขพาสปอร์ตของสหรัฐอเมริกา/UK</span><span class="sxs-lookup"><span data-stu-id="11cc9-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="11cc9-103">**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="11cc9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="11cc9-104">**ปัญหา DLP กับเลขพาสปอร์ตของสหรัฐอเมริกา/UK**</span><span class="sxs-lookup"><span data-stu-id="11cc9-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="11cc9-105">คุณมีปัญหาเกี่ยวกับการ **ป้องกันการสูญหายของข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่มี **หมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักร** เมื่อใช้ชนิดข้อมูลที่ละเอียดอ่อนของ DLP ใน O365 ใช่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="11cc9-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="11cc9-106">ถ้าเป็นเช่นนั้นตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จำเป็นสำหรับสิ่งที่นโยบาย DLP กำลังค้นหาเมื่อมีการประเมิน</span><span class="sxs-lookup"><span data-stu-id="11cc9-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="11cc9-107">ตัวอย่างเช่นสำหรับนโยบาย **หมายเลขหนังสือเดินทางสหรัฐอเมริกา/UK** ที่กำหนดค่าด้วยระดับความเชื่อมั่นของ๗๕% ต่อไปนี้จะถูกประเมินและต้องถูกตรวจพบสำหรับกฎที่จะทริกเกอร์</span><span class="sxs-lookup"><span data-stu-id="11cc9-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="11cc9-108">**[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** เก้าหลัก</span><span class="sxs-lookup"><span data-stu-id="11cc9-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="11cc9-109">**[ลวดลาย:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** ตัวเลขที่ติดต่อกันได้9ตัว</span><span class="sxs-lookup"><span data-stu-id="11cc9-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="11cc9-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** ไม่มี Checksum</span><span class="sxs-lookup"><span data-stu-id="11cc9-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="11cc9-111">**[ข้อกำหนด:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** นโยบาย DLP มีความมั่นใจ๗๕% ว่าจะตรวจพบข้อมูลที่เป็นความลับชนิดนี้ในกรณีที่มีอักขระ๓๐๐ที่อยู่ในความใกล้เคียง:</span><span class="sxs-lookup"><span data-stu-id="11cc9-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="11cc9-112">ฟังก์ชัน Func_usa_uk_passport ค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="11cc9-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="11cc9-113">พบคำสำคัญจาก Keyword_passport</span><span class="sxs-lookup"><span data-stu-id="11cc9-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="11cc9-114">ตัวอย่างเช่นตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับนโยบาย **หมายเลขหนังสือเดินทางสหรัฐอเมริกา/UK** : หมายเลขหนังสือเดินทางของสหรัฐอเมริกา๑๒๓๔๕๖๗๘๙</span><span class="sxs-lookup"><span data-stu-id="11cc9-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="11cc9-115">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จำเป็นสำหรับหมายเลขหนังสือเดินทางของสหรัฐอเมริกา/UK ที่จะถูกตรวจพบสำหรับเนื้อหาของคุณให้ดูส่วนต่อไปนี้ในบทความนี้: [ชนิดข้อมูลที่เป็นความลับของหมายเลขหนังสือเดินทางของสหรัฐอเมริกา/สหราชอาณาจักร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="11cc9-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="11cc9-116">การใช้ชนิดข้อมูลที่มีความสำคัญที่มีอยู่แล้วภายในที่แตกต่างกันให้ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งที่จำเป็นสำหรับชนิดอื่นๆ: [ชนิดข้อมูลที่เป็นความลับที่มีลักษณะสำหรับ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="11cc9-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  