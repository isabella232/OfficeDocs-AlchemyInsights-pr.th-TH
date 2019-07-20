---
title: เหมือนกับชื่อแฟ้มที่ดีที่สุดคือ
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
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800064"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="e9ebc-102">จำเป็นต้องใช้ Alchemy หัว H1, H2 ของไม่ทำงาน</span><span class="sxs-lookup"><span data-stu-id="e9ebc-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="e9ebc-103">แนวทางปฏิบัติและแนวทางในการเขียนแก้ Alchemy:</span><span class="sxs-lookup"><span data-stu-id="e9ebc-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="e9ebc-104">**ซ้อนความเข้าใจ Alchemy ในโฟลเดอร์**- นี้จะเป็นแบ่งโครงสร้าง url</span><span class="sxs-lookup"><span data-stu-id="e9ebc-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="e9ebc-105">เรากำลังค้นหาลงในการซ่อมแซมนี้</span><span class="sxs-lookup"><span data-stu-id="e9ebc-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="e9ebc-106">แฟ้มในโฟลเดอร์**AlchemyInsights**ที่ควรมีชื่อแฟ้มเล็ก ด้วยยัติภังค์สำหรับช่องว่างแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="e9ebc-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="e9ebc-107">***how-เพื่อเปิดใช้งานดำเนินคดีค้างไว้***</span><span class="sxs-lookup"><span data-stu-id="e9ebc-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="e9ebc-108">รวมหมายเลข ID ของกฎหรือกลุ่มจาก[เว็บไซต์คู่ค้า Alchemy](https://alchemyportal.azurewebsites.net)ในฟิลด์ ms.custom</span><span class="sxs-lookup"><span data-stu-id="e9ebc-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="e9ebc-109">ในอดีต</span><span class="sxs-lookup"><span data-stu-id="e9ebc-109">ex.</span></span> <span data-ttu-id="e9ebc-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="e9ebc-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="e9ebc-111">ใช้ส่วนเหลือของข้อมูลเมตาที่ด้านบนของแฟ้มนี้เป็นแม่แบบของคุณ</span><span class="sxs-lookup"><span data-stu-id="e9ebc-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="e9ebc-112">ใน[เว็บไซต์คู่ค้า Alchemy](https://alchemyportal.azurewebsites.net)นำทางลงไปส่วน**ลูกค้าช่วยเรื่อง:** และการใช้ที่ชี้เป็นการเริ่มต้นสำหรับชื่อเรื่อง H1 ของคุณสำหรับการช่วย</span><span class="sxs-lookup"><span data-stu-id="e9ebc-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="e9ebc-113">Alchemy ความเข้าใจต้องมี H1 เดียวเท่านั้นที่ด้านบน หรือพวกเขาจะเป็นแบ่งในการผลิต</span><span class="sxs-lookup"><span data-stu-id="e9ebc-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="e9ebc-114">H2s ไม่แสดงผลอย่างใดอย่างหนึ่งเพื่อใช้**เป็นตัวหนา**หรือแบบแผนอื่น ๆ เพื่อแสดงส่วนที่แยกต่างหาก</span><span class="sxs-lookup"><span data-stu-id="e9ebc-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="e9ebc-115">กรอกข้อมูลในตัวข้อความโดยใช้วัสดุแบบร่างในส่วนความเข้าใจลูกค้าของกฎ Alchemy หน้าถัดไป</span><span class="sxs-lookup"><span data-stu-id="e9ebc-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="e9ebc-116">รายการหัวข้อย่อยไม่มีปัญหา</span><span class="sxs-lookup"><span data-stu-id="e9ebc-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="e9ebc-117">รายการที่มีตัวเลขมากเกินไป</span><span class="sxs-lookup"><span data-stu-id="e9ebc-117">Numbered lists too</span></span>
    1. <span data-ttu-id="e9ebc-118">**ตัวหนา**และ*ตัวเอียง*จะ a-ok</span><span class="sxs-lookup"><span data-stu-id="e9ebc-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="e9ebc-119">การเชื่อมโยงควรจะเสมออย่างใดอย่างหนึ่ง **"การเชื่อมโยงไปยังเว็บ" / ภายนอก**หรือ**ความลึกเชื่อมโยงไปยังองค์ประกอบ UI**การเชื่อมโยงภายในไม่</span><span class="sxs-lookup"><span data-stu-id="e9ebc-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="e9ebc-120">รูปภาพจะไม่เป็นได้รับการสนับสนุนในขณะนี้ แต่ในแผนการทำงานนี้</span><span class="sxs-lookup"><span data-stu-id="e9ebc-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="e9ebc-121">และนี่คือจริง ๆ แล้วยาวเกินไปสักเล็กน้อย</span><span class="sxs-lookup"><span data-stu-id="e9ebc-121">And this is really already a bit too long.</span></span> <span data-ttu-id="e9ebc-122">แนวทางปฏิบัติที่ดีที่สุดคือ อักขระประมาณ 400---</span><span class="sxs-lookup"><span data-stu-id="e9ebc-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="e9ebc-123">หลังจากที่เนื้อหาของคุณมาพร้อม ดึงการถ่ายทอดสดสาขา</span><span class="sxs-lookup"><span data-stu-id="e9ebc-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="e9ebc-124">แล้ว ไปที่[เว็บไซต์คู่ค้า Alchemy](https://alchemyportal.azurewebsites.net)และป้อนชื่อแฟ้มลงในฟิลด์ url</span><span class="sxs-lookup"><span data-stu-id="e9ebc-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 