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
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697149"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="0501f-102">จำเป็นต้องใช้ Alchemy หัว H1, H2 ของไม่ทำงาน</span><span class="sxs-lookup"><span data-stu-id="0501f-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="0501f-103">แนวทางปฏิบัติและแนวทางในการเขียนแก้ Alchemy:</span><span class="sxs-lookup"><span data-stu-id="0501f-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="0501f-p101">**ซ้อนความเข้าใจ Alchemy ในโฟลเดอร์**- นี้จะเป็นแบ่งโครงสร้าง url เรากำลังค้นหาลงในการซ่อมแซมนี้</span><span class="sxs-lookup"><span data-stu-id="0501f-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="0501f-106">แฟ้มในโฟลเดอร์**AlchemyInsights**ควรมีกฎรหัสและชื่อของกฎจาก[เว็บไซต์คู่ค้า Alchemy](https://alchemyportal.azurewebsites.net)ในชื่อแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="0501f-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="0501f-p102">เช่น***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="0501f-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="0501f-p103">ใช้ข้อมูลเมตาที่ด้านบนของแฟ้มนี้เป็นแม่แบบของคุณ ไม่มีอะไรอื่นที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="0501f-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="0501f-111">ใน[เว็บไซต์คู่ค้า Alchemy](https://alchemyportal.azurewebsites.net)นำทางลงไปส่วน**ลูกค้าช่วยเรื่อง:** และการใช้ที่ชี้เป็นการเริ่มต้นสำหรับชื่อเรื่อง H1 ของคุณสำหรับการช่วย</span><span class="sxs-lookup"><span data-stu-id="0501f-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="0501f-p104">Alchemy ความเข้าใจต้องมี H1 เดียวเท่านั้นที่ด้านบน หรือพวกเขาจะเป็นแบ่งในการผลิต H2s ไม่แสดงผลอย่างใดอย่างหนึ่งเพื่อใช้**เป็นตัวหนา**หรือแบบแผนอื่น ๆ เพื่อแสดงส่วนที่แยกต่างหาก</span><span class="sxs-lookup"><span data-stu-id="0501f-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="0501f-114">กรอกข้อมูลในตัวข้อความโดยใช้วัสดุแบบร่างในส่วนความเข้าใจลูกค้าของกฎ Alchemy หน้าถัดไป</span><span class="sxs-lookup"><span data-stu-id="0501f-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="0501f-115">รายการหัวข้อย่อยไม่มีปัญหา</span><span class="sxs-lookup"><span data-stu-id="0501f-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="0501f-116">รายการที่มีตัวเลขมากเกินไป</span><span class="sxs-lookup"><span data-stu-id="0501f-116">Numbered lists too</span></span>
    1. <span data-ttu-id="0501f-117">**ตัวหนา**และ*ตัวเอียง*จะ a-ok</span><span class="sxs-lookup"><span data-stu-id="0501f-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="0501f-118">การเชื่อมโยงควรจะเสมออย่างใดอย่างหนึ่ง **"การเชื่อมโยงไปยังเว็บ" / ภายนอก**หรือ**ความลึกเชื่อมโยงไปยังองค์ประกอบ UI**การเชื่อมโยงภายในไม่</span><span class="sxs-lookup"><span data-stu-id="0501f-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="0501f-p105">และนี่คือจริง ๆ แล้วยาวเกินไปสักเล็กน้อย แนวทางปฏิบัติที่ดีที่สุดคือ อักขระประมาณ 400---</span><span class="sxs-lookup"><span data-stu-id="0501f-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="0501f-p106">หลังจากที่เนื้อหาของคุณมาพร้อม ดึงการถ่ายทอดสดสาขา แล้ว ไปที่[เว็บไซต์คู่ค้า Alchemy](https://alchemyportal.azurewebsites.net)และป้อนชื่อแฟ้มลงในฟิลด์ url ตรวจสอบว่า ช่วยตรวจทาน และเผยแพร่ข้อความว่า "ใช่" และจากนั้น คลิกกฎการปรับปรุง **(ซึ่งจะค้นหา prettier ในพอร์ทัล - ปล่อยเร็ว ๆ นี้รุ่นใหม่)** 
![ฟิลด์ url](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="0501f-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

