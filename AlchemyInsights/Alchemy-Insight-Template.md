---
title: เหมือนกับชื่อไฟล์ที่ดีที่สุด
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664153"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="9f891-102">"จำเป็นต้องใช้งานส่วนหัวของ H1, H2's ไม่ทำงาน"</span><span class="sxs-lookup"><span data-stu-id="9f891-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="9f891-103">แนวทางปฏิบัติและแนวทางปฏิบัติที่ดีที่สุดสำหรับการสร้างขลัง:</span><span class="sxs-lookup"><span data-stu-id="9f891-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="9f891-104">**อย่าทำรังข้อมูลเชิงลึกของขลังในโฟลเดอร์**-ซึ่งจะตัดโครงสร้าง url</span><span class="sxs-lookup"><span data-stu-id="9f891-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="9f891-105">เรากำลังค้นหาในการแก้ไขปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="9f891-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="9f891-106">ไฟล์ในโฟลเดอร์ **AlchemyInsights** ควรมีชื่อไฟล์ตัวพิมพ์เล็กที่มียัติภังค์สำหรับช่องว่าง ex</span><span class="sxs-lookup"><span data-stu-id="9f891-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="9f891-107">***วิธีการเปิดใช้งานการระงับการดำเนินคดี***</span><span class="sxs-lookup"><span data-stu-id="9f891-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="9f891-108">รวม ID กฎหรือ ID ของกลุ่มจาก [พอร์ทัลคู่ค้าที่ขลัง](https://alchemyportal.azurewebsites.net) ในเขตข้อมูลแบบกำหนดเองของ ms</span><span class="sxs-lookup"><span data-stu-id="9f891-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="9f891-109">ตัวอย่าง .</span><span class="sxs-lookup"><span data-stu-id="9f891-109">ex.</span></span> <span data-ttu-id="9f891-110">***ms ที่กำหนดเอง: ๑๐๐๐๒๑***</span><span class="sxs-lookup"><span data-stu-id="9f891-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="9f891-111">ใช้ metadata ที่เหลือที่ด้านบนของไฟล์นี้เป็นเทมเพลตของคุณ</span><span class="sxs-lookup"><span data-stu-id="9f891-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="9f891-112">ใน [พอร์ทัลคู่ค้าที่ขลัง](https://alchemyportal.azurewebsites.net)ให้นำทางไปยังหัวข้อข้อมูล **เชิงลึกของลูกค้าส่วน:** และใช้เป็นจุดเริ่มต้นสำหรับชื่อ H1 ของคุณสำหรับข้อมูลเชิงลึก</span><span class="sxs-lookup"><span data-stu-id="9f891-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="9f891-113">ข้อมูลเชิงลึกของขลังต้องมีเพียง H1 เดียวที่ด้านบนหรือพวกเขาจะแบ่งในการผลิต</span><span class="sxs-lookup"><span data-stu-id="9f891-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="9f891-114">ไม่มีการแสดงอย่างใดอย่างหนึ่งให้ใช้ตัว **หนา** หรือแบบแผนอื่นๆเพื่อแสดงส่วนที่แยกต่างหาก</span><span class="sxs-lookup"><span data-stu-id="9f891-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="9f891-115">ถัดไปให้กรอกข้อความเนื้อหาโดยใช้เนื้อหาแบบร่างในส่วนข้อมูลเชิงลึกของลูกค้าของหน้ากฎการขลัง</span><span class="sxs-lookup"><span data-stu-id="9f891-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="9f891-116">รายการสัญลักษณ์แสดงหัวข้อย่อยจะดี</span><span class="sxs-lookup"><span data-stu-id="9f891-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="9f891-117">รายการลำดับเลขเกินไป</span><span class="sxs-lookup"><span data-stu-id="9f891-117">Numbered lists too</span></span>
    1. <span data-ttu-id="9f891-118">ตัว**หนา**และตัว*เอียง*คือ a-ตกลง</span><span class="sxs-lookup"><span data-stu-id="9f891-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="9f891-119">ลิงก์ควรจะเป็น **"ลิงก์ไปยังเว็บ"/External** หรือ **ลิงก์ลึกไปยังองค์ประกอบ UI**ไม่ใช่ลิงก์ภายใน</span><span class="sxs-lookup"><span data-stu-id="9f891-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="9f891-120">รูปภาพไม่ได้รับการสนับสนุนอย่างเป็นทางการในขณะนี้แต่จะอยู่บนแผนการทำงาน</span><span class="sxs-lookup"><span data-stu-id="9f891-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="9f891-121">และนี่คือความยาวของบิตที่ยาวเกินไป</span><span class="sxs-lookup"><span data-stu-id="9f891-121">And this is really already a bit too long.</span></span> <span data-ttu-id="9f891-122">แนวทางปฏิบัติที่ดีที่สุดคือ---------------------------------อักขระ๔๐๐</span><span class="sxs-lookup"><span data-stu-id="9f891-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="9f891-123">เมื่อเนื้อหาของคุณพร้อมแล้วให้ดึงข้อมูลไปยังสาขาสด</span><span class="sxs-lookup"><span data-stu-id="9f891-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="9f891-124">จากนั้นไปที่ [พอร์ทัลคู่ค้าขลัง](https://alchemyportal.azurewebsites.net) แล้วใส่ชื่อไฟล์ลงในเขตข้อมูล url</span><span class="sxs-lookup"><span data-stu-id="9f891-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 