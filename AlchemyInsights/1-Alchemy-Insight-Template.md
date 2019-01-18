---
title: 'เป็นการดีที่สุดคือชื่อแฟ้มเดียวกัน [กฎ #-อธิบาย]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 9e2a369f4b1bf87da8b12224b5f6e8b1138db9dd
ms.sourcegitcommit: 59f8f84ab99bad3f9d26ee412d20dc36759e3e6e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2019
ms.locfileid: "28727542"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a><span data-ttu-id="c5a80-102">จำเป็นต้องใช้ลูกค้าหัน H1, H2 ไม่ทำงาน</span><span class="sxs-lookup"><span data-stu-id="c5a80-102">Required Customer Facing H1, H2 doesn't work</span></span>
<span data-ttu-id="c5a80-103">ตัวอย่างข้อความบล็อก - ทำตามคำแนะนำเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="c5a80-103">Example text block - follow these instructions:</span></span>

1. <span data-ttu-id="c5a80-104">แฟ้มในโฟลเดอร์**AlchemyInsights**ควรมีกฎรหัสและชื่อของกฎจาก[เว็บไซต์คู่ค้า Alchemy](https://alchemyportal.azurewebsites.net)ใน mane</span><span class="sxs-lookup"><span data-stu-id="c5a80-104">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the mane.</span></span>
    1. <span data-ttu-id="c5a80-p101">เช่น***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="c5a80-p101">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="c5a80-p102">ใช้ข้อมูลเมตาที่ด้านบนของแฟ้มนี้เป็นแม่แบบของคุณ ไม่มีอะไรอื่นที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="c5a80-p102">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="c5a80-109">ใน[เว็บไซต์คู่ค้า Alchemy](https://alchemyportal.azurewebsites.net)นำทางลงไปส่วน**ลูกค้าช่วยเรื่อง:** และการใช้ที่ชี้เป็นการเริ่มต้นสำหรับชื่อเรื่อง H1 ของคุณสำหรับการช่วย</span><span class="sxs-lookup"><span data-stu-id="c5a80-109">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="c5a80-p103">Alchemy ความเข้าใจต้องมี H1 เดียวเท่านั้นที่ด้านบน หรือพวกเขาจะเป็นแบ่งในการผลิต H2s ไม่แสดงผลอย่างใดอย่างหนึ่งเพื่อใช้**เป็นตัวหนา**หรือแบบแผนอื่น ๆ เพื่อแสดงส่วนที่แยกต่างหาก</span><span class="sxs-lookup"><span data-stu-id="c5a80-p103">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="c5a80-112">กรอกข้อมูลในตัวข้อความโดยใช้วัสดุแบบร่างในส่วนความเข้าใจลูกค้าของกฎ Alchemy หน้าถัดไป</span><span class="sxs-lookup"><span data-stu-id="c5a80-112">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="c5a80-113">รายการหัวข้อย่อยไม่มีปัญหา</span><span class="sxs-lookup"><span data-stu-id="c5a80-113">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="c5a80-114">รายการที่มีตัวเลขมากเกินไป</span><span class="sxs-lookup"><span data-stu-id="c5a80-114">Numbered lists too</span></span>
    1. <span data-ttu-id="c5a80-115">**ตัวหนา**และ*ตัวเอียง*จะ a-ok</span><span class="sxs-lookup"><span data-stu-id="c5a80-115">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="c5a80-116">การเชื่อมโยงควรจะเสมออย่างใดอย่างหนึ่ง **"การเชื่อมโยงไปยังเว็บ" / ภายนอก**หรือ**ความลึกเชื่อมโยงไปยังองค์ประกอบ UI**การเชื่อมโยงภายในไม่</span><span class="sxs-lookup"><span data-stu-id="c5a80-116">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="c5a80-p104">และนี่คือจริง ๆ แล้วยาวเกินไปสักเล็กน้อย แนวทางปฏิบัติที่ดีที่สุดคือ อักขระประมาณ 400---</span><span class="sxs-lookup"><span data-stu-id="c5a80-p104">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>