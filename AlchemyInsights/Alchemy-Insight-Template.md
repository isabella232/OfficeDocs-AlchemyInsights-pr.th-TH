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
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676552"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="3d96b-102">ต้องเล่นแร่แปรธาตุส่วนหัว H1, H2 ไม่ทํางาน</span><span class="sxs-lookup"><span data-stu-id="3d96b-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="3d96b-103">แนวทางปฏิบัติและแนวทางที่ดีที่สุดในการเขียนการเล่นแร่แปรธาตุ:</span><span class="sxs-lookup"><span data-stu-id="3d96b-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="3d96b-104">**อย่ารังขลังเจาะลึกในโฟลเดอร์**-- นี้จะทําลายโครงสร้าง URL</span><span class="sxs-lookup"><span data-stu-id="3d96b-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="3d96b-105">เรากําลังตามหาการแก้ไขนี้</span><span class="sxs-lookup"><span data-stu-id="3d96b-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="3d96b-106">แฟ้มในโฟลเดอร์**AlchemyInsights**ควรมีชื่อไฟล์ตัวพิมพ์เล็กที่มีเครื่องหมายยัติภังค์สําหรับเว้นวรรค</span><span class="sxs-lookup"><span data-stu-id="3d96b-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="3d96b-107">***วิธีการ - เพื่อเปิดใช้งานการดําเนินคดีถือ***</span><span class="sxs-lookup"><span data-stu-id="3d96b-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="3d96b-108">รวมรหัสกฎหรือ ID ที่ฝากข้อมูลจากเว็บไซต์[คู่ค้าของการเล่นแร่แปรธาตุ](https://alchemyportal.azurewebsites.net)ในฟิลด์ ms.custom</span><span class="sxs-lookup"><span data-stu-id="3d96b-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="3d96b-109">เช่น</span><span class="sxs-lookup"><span data-stu-id="3d96b-109">ex.</span></span> <span data-ttu-id="3d96b-110">***msของที่กําหนดเอง: 100021***</span><span class="sxs-lookup"><span data-stu-id="3d96b-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="3d96b-111">ใช้ข้อมูลเมตาที่เหลือที่ด้านบนของแฟ้มนี้เป็นแม่แบบของคุณ</span><span class="sxs-lookup"><span data-stu-id="3d96b-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="3d96b-112">ใน[พอร์ทัลพันธมิตรการเล่นแร่แปรธาตุ](https://alchemyportal.azurewebsites.net)ให้นําทางลงไปที่ส่วน**หัวข้อข้อมูลเชิงลึกของลูกค้า:** และใช้เป็นจุดเริ่มต้นสําหรับชื่อเรื่อง H1 ของคุณสําหรับข้อมูลเชิงลึก</span><span class="sxs-lookup"><span data-stu-id="3d96b-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="3d96b-113">ข้อมูลเชิงลึกของการเล่นแร่แปรธาตุต้องมีเพียงหนึ่ง H1 ที่ด้านบนหรือพวกเขาจะทําลายในการผลิต</span><span class="sxs-lookup"><span data-stu-id="3d96b-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="3d96b-114">H2s ไม่แสดงให้ใช้**แบบตัวหนา**หรืออนุสัญญาอื่นๆ เพื่อบ่งบอกถึงส่วนที่แยกต่างหาก</span><span class="sxs-lookup"><span data-stu-id="3d96b-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="3d96b-115">จากนั้น ให้กรอกข้อมูลในเนื้อความโดยใช้เนื้อหาร่างในส่วน Customer Insights ของหน้ากฎการเล่นแร่แปรธาตุ</span><span class="sxs-lookup"><span data-stu-id="3d96b-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="3d96b-116">รายการสัญลักษณ์แสดงหัวข้อย่อยจะปรับได้</span><span class="sxs-lookup"><span data-stu-id="3d96b-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="3d96b-117">รายการที่มีหมายเลขเกินไป</span><span class="sxs-lookup"><span data-stu-id="3d96b-117">Numbered lists too</span></span>
    1. <span data-ttu-id="3d96b-118">**ตัวหนา**และ*ตัวเอียง*เป็น - ok</span><span class="sxs-lookup"><span data-stu-id="3d96b-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="3d96b-119">ลิงก์ควรเป็น**ทั้ง"การเชื่อมโยงไปยังเว็บ"/ภายนอก**หรือ**การเชื่อมโยงลึกไปยังองค์ประกอบ UI**, ไม่เชื่อมโยงภายใน</span><span class="sxs-lookup"><span data-stu-id="3d96b-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="3d96b-120">รูปภาพไม่ได้รับการสนับสนุนอย่างเป็นทางการในเวลานี้ แต่ในแผนงาน</span><span class="sxs-lookup"><span data-stu-id="3d96b-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="3d96b-121">และนี่ก็นานเกินไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="3d96b-121">And this is really already a bit too long.</span></span> <span data-ttu-id="3d96b-122">แนวทางปฏิบัติที่ดีที่สุดคือประมาณ 400 อักขระ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="3d96b-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="3d96b-123">เมื่อเนื้อหาของคุณพร้อมแล้วให้ดึงไปที่สาขาสด</span><span class="sxs-lookup"><span data-stu-id="3d96b-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="3d96b-124">จากนั้น ไปที่[พอร์ทัลพันธมิตรการเล่นแร่แปรธาตุ](https://alchemyportal.azurewebsites.net)และป้อนชื่อไฟล์ลงในช่อง url</span><span class="sxs-lookup"><span data-stu-id="3d96b-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 