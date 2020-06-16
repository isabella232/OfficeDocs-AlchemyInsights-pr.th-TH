---
title: เช่นเดียวกับชื่อไฟล์ที่ดีที่สุด
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750989"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="be92c-102">"ส่วนหัวขลังที่จําเป็น H1, H2 ไม่ทํางาน."</span><span class="sxs-lookup"><span data-stu-id="be92c-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="be92c-103">แนวทางปฏิบัติที่ดีที่สุดและแนวทางสําหรับการเขียนการเล่นแร่แปรธาตุ:</span><span class="sxs-lookup"><span data-stu-id="be92c-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="be92c-104">**ไม่รังลึกขลังในโฟลเดอร์**-- นี้จะทําลายโครงสร้าง URL</span><span class="sxs-lookup"><span data-stu-id="be92c-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="be92c-105">เรากําลังค้นหาการแก้ไขนี้</span><span class="sxs-lookup"><span data-stu-id="be92c-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="be92c-106">ไฟล์ในโฟลเดอร์**AlchemyInsights**ควรมีชื่อไฟล์ตัวพิมพ์เล็กที่มีเครื่องหมายยัติภังค์สําหรับเว้นวรรค</span><span class="sxs-lookup"><span data-stu-id="be92c-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="be92c-107">***วิธีการเปิดใช้งานการดําเนินคดี-ระงับ***</span><span class="sxs-lookup"><span data-stu-id="be92c-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="be92c-108">ใส่รหัสกฎหรือรหัสบัคเก็ตจาก[พอร์ทัลพันธมิตรการเล่นแร่แปรธาตุ](https://alchemyportal.azurewebsites.net)ในฟิลด์ ms.custom</span><span class="sxs-lookup"><span data-stu-id="be92c-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="be92c-109">เช่น</span><span class="sxs-lookup"><span data-stu-id="be92c-109">ex.</span></span> <span data-ttu-id="be92c-110">***msของที่กําหนดเอง: 100021***</span><span class="sxs-lookup"><span data-stu-id="be92c-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="be92c-111">ใช้ข้อมูลเมตาที่เหลือที่ด้านบนของแฟ้มนี้เป็นแม่แบบของคุณ</span><span class="sxs-lookup"><span data-stu-id="be92c-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="be92c-112">ใน[พอร์ทัลพันธมิตรขลัง](https://alchemyportal.azurewebsites.net), ลงไปที่ส่วน**ลูกค้า Insight Title:** และใช้ที่เป็นจุดเริ่มต้นสําหรับชื่อ H1 ของคุณสําหรับข้อมูลเชิงลึก.</span><span class="sxs-lookup"><span data-stu-id="be92c-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="be92c-113">ข้อมูลเชิงลึกการเล่นแร่แปรธาตุต้องมีเพียงหนึ่ง H1 ที่ด้านบนหรือพวกเขาจะทําลายในการผลิต</span><span class="sxs-lookup"><span data-stu-id="be92c-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="be92c-114">H2s ไม่แสดงอย่างใดอย่างหนึ่งดังนั้นใช้**แบบแผนตัวหนา**หรืออื่น ๆ เพื่อมีความหมายแยกส่วน.</span><span class="sxs-lookup"><span data-stu-id="be92c-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="be92c-115">จากนั้นกรอกข้อความเนื้อหาโดยใช้วัสดุร่างในส่วนข้อมูลเชิงลึกของลูกค้าในหน้ากฎการเล่นแร่แปรธาตุ</span><span class="sxs-lookup"><span data-stu-id="be92c-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="be92c-116">รายการสัญลักษณ์แสดงหัวข้อย่อยจะปรับ</span><span class="sxs-lookup"><span data-stu-id="be92c-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="be92c-117">รายการลําดับเลขเกินไป</span><span class="sxs-lookup"><span data-stu-id="be92c-117">Numbered lists too</span></span>
    1. <span data-ttu-id="be92c-118">**ตัวหนา**และ*ตัวเอียง*เป็น ok</span><span class="sxs-lookup"><span data-stu-id="be92c-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="be92c-119">ลิงค์ควรเป็น**ทั้ง"เชื่อมโยงไปยังเว็บ"/ภายนอก**หรือ**ลึกเชื่อมโยงไปยังองค์ประกอบ UI,** ไม่เชื่อมโยงภายใน</span><span class="sxs-lookup"><span data-stu-id="be92c-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="be92c-120">รูปภาพไม่ได้รับการสนับสนุนอย่างเป็นทางการในขณะนี้ แต่เป็นแผนงาน</span><span class="sxs-lookup"><span data-stu-id="be92c-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="be92c-121">และนี่ก็ยาวเกินไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="be92c-121">And this is really already a bit too long.</span></span> <span data-ttu-id="be92c-122">แนวทางปฏิบัติที่ดีที่สุดคือประมาณ 400 ตัวอักษร---------------------------------</span><span class="sxs-lookup"><span data-stu-id="be92c-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="be92c-123">เมื่อเนื้อหาของคุณพร้อมแล้ว ให้ดึงเนื้อหานั้นไปยังสาขาที่ถ่ายทอดสด</span><span class="sxs-lookup"><span data-stu-id="be92c-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="be92c-124">จากนั้นไปที่[พอร์ทัลพันธมิตรการเล่นแร่แปรธาตุ](https://alchemyportal.azurewebsites.net)และป้อนชื่อไฟล์ลงในช่อง URL</span><span class="sxs-lookup"><span data-stu-id="be92c-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 