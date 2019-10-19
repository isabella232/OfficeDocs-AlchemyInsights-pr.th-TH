---
title: เหมือนกับชื่อไฟล์ที่ดีที่สุด
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "35800064"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="b6958-102">ส่วนหัวที่ต้องใช้ในการเล่นแร่แปรธาตุ H1, H2's ไม่ทำงาน</span><span class="sxs-lookup"><span data-stu-id="b6958-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="b6958-103">แนวทางปฏิบัติที่ดีที่สุดสำหรับการเขียนแก้การเล่นแร่แปรธาตุ:</span><span class="sxs-lookup"><span data-stu-id="b6958-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="b6958-104">**อย่าซ้อนข้อมูลเชิงลึกในการเล่นแร่แปรธาตุในโฟลเดอร์**-นี้จะทำลายโครงสร้างของ url</span><span class="sxs-lookup"><span data-stu-id="b6958-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="b6958-105">เรากำลังมองหาการแก้ไขปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="b6958-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="b6958-106">ไฟล์ในโฟลเดอร์**AlchemyInsights**ควรมีชื่อไฟล์ตัวพิมพ์เล็กที่มียัติภังค์สำหรับช่องว่าง ex</span><span class="sxs-lookup"><span data-stu-id="b6958-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="b6958-107">***วิธีการเปิดใช้งานการดำเนินคดีค้างไว้***</span><span class="sxs-lookup"><span data-stu-id="b6958-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="b6958-108">รวมรหัสกฎหรือรหัสกลุ่มจาก[พอร์ทัลพาร์ทเนอร์การเล่นแร่แปรธาตุ](https://alchemyportal.azurewebsites.net)ในฟิลด์แบบกำหนดเองของ ms</span><span class="sxs-lookup"><span data-stu-id="b6958-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="b6958-109">เช่น</span><span class="sxs-lookup"><span data-stu-id="b6958-109">ex.</span></span> <span data-ttu-id="b6958-110">***นางสาวกำหนดเอง: ๑๐๐๐๒๑***</span><span class="sxs-lookup"><span data-stu-id="b6958-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="b6958-111">ใช้ส่วนที่เหลือของข้อมูลเมตาที่ด้านบนของแฟ้มนี้เป็นแม่แบบของคุณ</span><span class="sxs-lookup"><span data-stu-id="b6958-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="b6958-112">ใน[พอร์ทัลพาร์ทเนอร์การเล่นแร่แปรธาตุ](https://alchemyportal.azurewebsites.net)ให้นำทางลงไปที่ส่วน**หัวข้อเชิงลึกของลูกค้า:** และใช้ที่เป็นจุดเริ่มต้นสำหรับชื่อ H1 ของคุณสำหรับข้อมูลเชิงลึก</span><span class="sxs-lookup"><span data-stu-id="b6958-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="b6958-113">ข้อมูลเชิงลึกในการเล่นแร่แปรธาตุต้องมีเพียงหนึ่ง H1 ที่ด้านบนหรือพวกเขาจะทำลายในการผลิต</span><span class="sxs-lookup"><span data-stu-id="b6958-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="b6958-114">H2s ไม่แสดงให้ใช้แบบตัว**หนา**หรือแบบอื่นเพื่อแสดงถึงส่วนที่แยกต่างหาก</span><span class="sxs-lookup"><span data-stu-id="b6958-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="b6958-115">จากนั้นให้กรอกข้อความในเนื้อหาโดยใช้เนื้อหาแบบร่างในส่วนข้อมูลเชิงลึกของลูกค้าของหน้ากฎการเล่นแร่แปรธาตุ</span><span class="sxs-lookup"><span data-stu-id="b6958-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="b6958-116">รายการสัญลักษณ์แสดงหัวข้อย่อยจะดี</span><span class="sxs-lookup"><span data-stu-id="b6958-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="b6958-117">รายการลำดับเลขเกินไป</span><span class="sxs-lookup"><span data-stu-id="b6958-117">Numbered lists too</span></span>
    1. <span data-ttu-id="b6958-118">**หนา**และตัว*เอียง*เป็น a-ok</span><span class="sxs-lookup"><span data-stu-id="b6958-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="b6958-119">การเชื่อมโยงควรจะเป็น **"เชื่อมโยงไปยังเว็บ"/ภายนอก**หรือ**ลึกเชื่อมโยงไปยังองค์ประกอบ UI**ไม่ใช่การเชื่อมโยงภายใน</span><span class="sxs-lookup"><span data-stu-id="b6958-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="b6958-120">รูปภาพไม่ได้รับการสนับสนุนอย่างเป็นทางการในขณะนี้แต่ก็อยู่บนแผนการทำงาน</span><span class="sxs-lookup"><span data-stu-id="b6958-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="b6958-121">และนี่เป็นเรื่องที่ยาวเกินไป</span><span class="sxs-lookup"><span data-stu-id="b6958-121">And this is really already a bit too long.</span></span> <span data-ttu-id="b6958-122">แนวทางปฏิบัติที่ดีที่สุดคือประมาณ๔๐๐อักขระ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="b6958-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="b6958-123">เมื่อเนื้อหาของคุณพร้อมแล้วให้ดึงไปยังสาขาที่มีชีวิตอยู่</span><span class="sxs-lookup"><span data-stu-id="b6958-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="b6958-124">จากนั้นไปที่[พอร์ทัลพาร์ทเนอร์การเล่นแร่แปรธาตุ](https://alchemyportal.azurewebsites.net)และป้อนชื่อไฟล์ลงในช่อง url</span><span class="sxs-lookup"><span data-stu-id="b6958-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 