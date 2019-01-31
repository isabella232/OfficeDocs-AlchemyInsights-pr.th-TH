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
ms.openlocfilehash: 1bb1cb35f06e16a2dc85b7e2642b9fa0d203945e
ms.sourcegitcommit: b032c2ac45540b1eb5dd68a4ec7ce1a5d6922f0e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662949"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a><span data-ttu-id="f48b6-102">จำเป็นต้องใช้ลูกค้าหัน H1, H2 ไม่ทำงาน</span><span class="sxs-lookup"><span data-stu-id="f48b6-102">Required Customer Facing H1, H2 doesn't work</span></span>
<span data-ttu-id="f48b6-103">ตัวอย่างข้อความบล็อก - ทำตามคำแนะนำเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="f48b6-103">Example text block - follow these instructions:</span></span>

1. <span data-ttu-id="f48b6-104">แฟ้มในโฟลเดอร์**AlchemyInsights**ควรมีกฎรหัสและชื่อของกฎจาก[เว็บไซต์คู่ค้า Alchemy](https://alchemyportal.azurewebsites.net)ในชื่อแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="f48b6-104">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="f48b6-p101">เช่น***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="f48b6-p101">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="f48b6-p102">ใช้ข้อมูลเมตาที่ด้านบนของแฟ้มนี้เป็นแม่แบบของคุณ ไม่มีอะไรอื่นที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="f48b6-p102">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="f48b6-109">ใน[เว็บไซต์คู่ค้า Alchemy](https://alchemyportal.azurewebsites.net)นำทางลงไปส่วน**ลูกค้าช่วยเรื่อง:** และการใช้ที่ชี้เป็นการเริ่มต้นสำหรับชื่อเรื่อง H1 ของคุณสำหรับการช่วย</span><span class="sxs-lookup"><span data-stu-id="f48b6-109">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="f48b6-p103">Alchemy ความเข้าใจต้องมี H1 เดียวเท่านั้นที่ด้านบน หรือพวกเขาจะเป็นแบ่งในการผลิต H2s ไม่แสดงผลอย่างใดอย่างหนึ่งเพื่อใช้**เป็นตัวหนา**หรือแบบแผนอื่น ๆ เพื่อแสดงส่วนที่แยกต่างหาก</span><span class="sxs-lookup"><span data-stu-id="f48b6-p103">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="f48b6-112">กรอกข้อมูลในตัวข้อความโดยใช้วัสดุแบบร่างในส่วนความเข้าใจลูกค้าของกฎ Alchemy หน้าถัดไป</span><span class="sxs-lookup"><span data-stu-id="f48b6-112">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="f48b6-113">รายการหัวข้อย่อยไม่มีปัญหา</span><span class="sxs-lookup"><span data-stu-id="f48b6-113">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="f48b6-114">รายการที่มีตัวเลขมากเกินไป</span><span class="sxs-lookup"><span data-stu-id="f48b6-114">Numbered lists too</span></span>
    1. <span data-ttu-id="f48b6-115">**ตัวหนา**และ*ตัวเอียง*จะ a-ok</span><span class="sxs-lookup"><span data-stu-id="f48b6-115">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="f48b6-116">การเชื่อมโยงควรจะเสมออย่างใดอย่างหนึ่ง **"การเชื่อมโยงไปยังเว็บ" / ภายนอก**หรือ**ความลึกเชื่อมโยงไปยังองค์ประกอบ UI**การเชื่อมโยงภายในไม่</span><span class="sxs-lookup"><span data-stu-id="f48b6-116">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="f48b6-p104">และนี่คือจริง ๆ แล้วยาวเกินไปสักเล็กน้อย แนวทางปฏิบัติที่ดีที่สุดคือ อักขระประมาณ 400---</span><span class="sxs-lookup"><span data-stu-id="f48b6-p104">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="f48b6-p105">หลังจากที่เนื้อหาของคุณมาพร้อม ดึงการถ่ายทอดสดสาขา แล้ว ไปที่[เว็บไซต์คู่ค้า Alchemy](https://alchemyportal.azurewebsites.net)และป้อนชื่อแฟ้มลงในฟิลด์ url ตรวจสอบว่า ช่วยตรวจทาน และเผยแพร่ข้อความว่า "ใช่" และจากนั้น คลิกกฎการปรับปรุง (ซึ่งจะค้นหา prettier ในพอร์ทัล - ปล่อยเร็ว ๆ นี้รุ่นใหม่)</span><span class="sxs-lookup"><span data-stu-id="f48b6-p105">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. (This will look prettier in the new version of the portal - releasing soon.)</span></span>

![ฟิลด์ url](media/for-content-team.PNG)

