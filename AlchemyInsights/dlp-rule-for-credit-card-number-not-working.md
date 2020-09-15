---
title: กฎ DLP สำหรับหมายเลขบัตรเครดิตไม่ทำงาน
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679460"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="0ad79-102">ปัญหา DLP ที่มีหมายเลขบัตรเครดิต</span><span class="sxs-lookup"><span data-stu-id="0ad79-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="0ad79-103">**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="0ad79-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="0ad79-104">**ปัญหา DLP ที่มีหมายเลขบัตรเครดิต**</span><span class="sxs-lookup"><span data-stu-id="0ad79-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="0ad79-105">คุณมีปัญหาเกี่ยวกับการ **ป้องกันการสูญหายของข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่มี **หมายเลขบัตรเครดิต** เมื่อใช้ชนิดข้อมูลที่ละเอียดอ่อนของ DLP ใน O365 ใช่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="0ad79-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="0ad79-106">ถ้าเป็นเช่นนั้นตรวจสอบให้แน่ใจว่าเนื้อหาของคุณมีข้อมูลที่จำเป็นในการทริกเกอร์นโยบาย DLP เมื่อถูกประเมิน</span><span class="sxs-lookup"><span data-stu-id="0ad79-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="0ad79-107">ตัวอย่างเช่นสำหรับ **นโยบายบัตรเครดิต** ที่กำหนดค่าด้วยระดับความเชื่อมั่นของ๘๕% รายการต่อไปนี้จะถูกประเมินและต้องถูกตรวจพบสำหรับกฎที่จะทริกเกอร์:</span><span class="sxs-lookup"><span data-stu-id="0ad79-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="0ad79-108">**[รูปแบบ:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** ตัวเลข16หลักที่สามารถจัดรูปแบบหรือจัดรูปแบบ (dddddddddddddddd) และต้องผ่านการทดสอบ Luhn</span><span class="sxs-lookup"><span data-stu-id="0ad79-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="0ad79-109">**[ลวดลาย:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** รูปแบบที่มีความซับซ้อนและมีประสิทธิภาพมากที่ตรวจจับบัตรจากแบรนด์หลักๆทั้งหมดทั่วโลกรวมถึงวีซ่ามาสเตอร์การ์ดค้นพบบัตรซีเจซี, American Express, บัตรของขวัญและบัตร diner</span><span class="sxs-lookup"><span data-stu-id="0ad79-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="0ad79-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** ใช่ Luhn checksum</span><span class="sxs-lookup"><span data-stu-id="0ad79-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="0ad79-111">**[ข้อกำหนด:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** นโยบาย DLP มีความมั่นใจ๘๕% ว่าจะตรวจพบข้อมูลที่เป็นความลับชนิดนี้ในกรณีที่มีอักขระ๓๐๐ที่อยู่ในความใกล้เคียง:</span><span class="sxs-lookup"><span data-stu-id="0ad79-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="0ad79-112">ฟังก์ชัน Func_credit_card ค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="0ad79-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="0ad79-113">อย่างใดอย่างหนึ่งต่อไปนี้เป็นจริง:</span><span class="sxs-lookup"><span data-stu-id="0ad79-113">One of the following is true:</span></span>

  - <span data-ttu-id="0ad79-114">พบคำสำคัญจาก Keyword_cc_verification</span><span class="sxs-lookup"><span data-stu-id="0ad79-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="0ad79-115">พบคำสำคัญจาก Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="0ad79-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="0ad79-116">ฟังก์ชัน Func_expiration_date ค้นหาวันที่ในรูปแบบวันที่ที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="0ad79-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="0ad79-117">Checksum ที่ผ่านการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="0ad79-117">The checksum passes</span></span>

    <span data-ttu-id="0ad79-118">ตัวอย่างเช่นตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับนโยบายหมายเลขบัตรเครดิต DLP:</span><span class="sxs-lookup"><span data-stu-id="0ad79-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="0ad79-119">วีซ่า: ๔๔๘๕๓๖๔๗๓๙๕๒๗๓๕๒</span><span class="sxs-lookup"><span data-stu-id="0ad79-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="0ad79-120">หมดอายุ: 2/2009</span><span class="sxs-lookup"><span data-stu-id="0ad79-120">Expires: 2/2009</span></span>

<span data-ttu-id="0ad79-121">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งที่จำเป็นสำหรับ **หมายเลขบัตรเครดิต** ที่จะถูกตรวจพบสำหรับเนื้อหาของคุณให้ดูส่วนต่อไปนี้ในบทความนี้: [ชนิดข้อมูลที่เป็นความลับของการค้นหาบัตรเครดิต #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="0ad79-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="0ad79-122">การใช้ชนิดข้อมูลที่มีความสำคัญที่มีอยู่แล้วภายในที่แตกต่างกันให้ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งที่จำเป็นสำหรับชนิดอื่นๆ: [ชนิดข้อมูลที่เป็นความลับที่มีลักษณะสำหรับ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="0ad79-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  