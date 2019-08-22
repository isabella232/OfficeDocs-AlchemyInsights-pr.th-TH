---
title: กฎ DLP สำหรับหมายเลขบัตรเครดิตที่ไม่ทำงาน
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
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529974"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="a3b0d-102">การตัดสินค้าจากคลัง DLP ด้วยหมายเลขบัตรเครดิต</span><span class="sxs-lookup"><span data-stu-id="a3b0d-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="a3b0d-103">คุณกำลังมีปัญหากับ**การป้องกันการสูญเสียข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่ประกอบด้วยหมาย**เลขบัตรเครดิต**เมื่อใช้ชนิดข้อมูลที่เป็นความลับ DLP ใน O365 หรือไม่</span><span class="sxs-lookup"><span data-stu-id="a3b0d-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a3b0d-104">ถ้าเป็นเช่นนั้น ให้แน่ใจว่า เนื้อหาของคุณประกอบด้วยข้อมูลที่จำเป็นเพื่อทริกเกอร์นโยบาย DLP เมื่อถูกประเมิน</span><span class="sxs-lookup"><span data-stu-id="a3b0d-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="a3b0d-105">ตัวอย่างเช่น สำหรับ**บัตรเครดิตนโยบาย**การตั้งค่าคอนฟิก ด้วยระดับความเชื่อมั่นของ 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบกฎเพื่อทริกเกอร์:</span><span class="sxs-lookup"><span data-stu-id="a3b0d-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a3b0d-106">**[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 หลักซึ่งการจัดรูปแบบหรือไม่จัดรูปแบบ (dddddddddddddddd) และต้องผ่านการทดสอบ Luhn</span><span class="sxs-lookup"><span data-stu-id="a3b0d-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="a3b0d-107">**[รูปแบบ:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** รูปแบบที่สมบูรณ์ และซับซ้อนมากที่ตรวจพบการ์ดจากทั้งหมดหลักยี่ห้อทั่วโลก รวมทั้งวีซ่า มาสเตอร์การ์ด ค้นหาบัตร JCB อเมริกันเอ็กซ์เพรส บัตรของขวัญ และบัตร diner</span><span class="sxs-lookup"><span data-stu-id="a3b0d-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="a3b0d-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** ใช่ ตัวนับไว้ Luhn</span><span class="sxs-lookup"><span data-stu-id="a3b0d-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="a3b0d-109">**[คำนิยาม:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** นโยบาย DLP คือ 85% มั่นใจจะได้ตรวจพบชนิดข้อมูลที่เป็นความลับนี้ if ภายในมีความใกล้เคียง 300 อักขระ:</span><span class="sxs-lookup"><span data-stu-id="a3b0d-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a3b0d-110">ฟังก์ชัน Func_credit_card ค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="a3b0d-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="a3b0d-111">ต่อไปนี้เป็นจริง:</span><span class="sxs-lookup"><span data-stu-id="a3b0d-111">One of the following is true:</span></span>

  - <span data-ttu-id="a3b0d-112">พบคำสำคัญจาก Keyword_cc_verification</span><span class="sxs-lookup"><span data-stu-id="a3b0d-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="a3b0d-113">พบคำสำคัญจาก Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="a3b0d-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="a3b0d-114">ฟังก์ชัน Func_expiration_date ค้นหาวันที่ในรูปแบบวันที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="a3b0d-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="a3b0d-115">Checksum ผ่านไป</span><span class="sxs-lookup"><span data-stu-id="a3b0d-115">The checksum passes</span></span>

    <span data-ttu-id="a3b0d-116">ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับนโยบาย DLP หมายเลขบัตรเครดิต:</span><span class="sxs-lookup"><span data-stu-id="a3b0d-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="a3b0d-117">วีซ่า: การ 7352 3952 3647 4485</span><span class="sxs-lookup"><span data-stu-id="a3b0d-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="a3b0d-118">หมดอายุ: 2/2009</span><span class="sxs-lookup"><span data-stu-id="a3b0d-118">Expires: 2/2009</span></span>

<span data-ttu-id="a3b0d-119">สำหรับข้อมูลเพิ่มเติมบนสิ่งจำเป็นสำหรับ**หมายเลขบัตรเครดิต**สามารถตรวจพบคอมพิวเตอร์สำหรับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[สิ่งสำคัญชนิดข้อมูลค้นหาบัตรเครดิต #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="a3b0d-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="a3b0d-120">โดยใช้ชนิดข้อมูลที่สำคัญในตัวแตกต่างกัน ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งจำเป็นสำหรับชนิดอื่น ๆ:[สิ่งสำคัญชนิดข้อมูลค้นหา](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a3b0d-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  