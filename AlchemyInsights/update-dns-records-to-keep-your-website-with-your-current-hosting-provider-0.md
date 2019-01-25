---
title: อัพเดตเรกคอร์ด DNS จะเก็บเว็บไซต์ของคุณกับผู้ให้บริการจัดการโฮสต์สำหรับปัจจุบัน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493466"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="bed07-102">อัพเดตเรกคอร์ด DNS จะเก็บเว็บไซต์ของคุณกับผู้ให้บริการจัดการโฮสต์สำหรับปัจจุบัน</span><span class="sxs-lookup"><span data-stu-id="bed07-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="bed07-103">ในหน้า[โดเมน](https://portal.office.com/adminportal/home#/Domains)ในรายการโดเมน เลือกโดเมนคุณกำลังใช้สำหรับเว็บไซต์ของคุณ จากนั้น**ตั้งค่า DNS**ในบานหน้าต่างจัดการ</span><span class="sxs-lookup"><span data-stu-id="bed07-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="bed07-104">เลือก **+ เรกคอร์ดแบบกำหนดเองใหม่**และป้อนข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="bed07-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="bed07-105">ป้อน**ชนิดของ DNS** : **(ที่อยู่)**</span><span class="sxs-lookup"><span data-stu-id="bed07-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="bed07-106">สำหรับ**ชื่อโฮสต์หรือนามแฝง**พิมพ์ต่อไปนี้:**@**</span><span class="sxs-lookup"><span data-stu-id="bed07-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="bed07-107">สำหรับ**ที่อยู่ IP**พิมพ์อยู่ IP แบบคงที่สำหรับเว็บไซต์ของคุณซึ่งจะเป็นอยู่ในขณะนี้โฮสต์ (ตัวอย่างเช่น 172.16.140.1)</span><span class="sxs-lookup"><span data-stu-id="bed07-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="bed07-p101">ซึ่งต้องเป็นที่อยู่ IP แบบ*คงที่*สำหรับเว็บไซต์ ไม่เป็น*แบบไดนามิก*ที่อยู่ IP ตรวจสอบกับไซต์ที่เป็นโฮสต์เว็บไซต์ของคุณเพื่อให้แน่ใจว่า คุณสามารถรับที่อยู่ IP แบบคงที่สำหรับเว็บไซต์สาธารณะของคุณ</span><span class="sxs-lookup"><span data-stu-id="bed07-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="bed07-110">เลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="bed07-110">Select **Save**.</span></span> 
    
<span data-ttu-id="bed07-111">นอกจากนี้ คุณสามารถสร้างระเบียน CNAME เพื่อช่วยลูกค้าในการค้นหาเว็บไซต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="bed07-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="bed07-112">เลือก **+ เรกคอร์ดแบบกำหนดเองใหม่**และป้อนข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="bed07-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="bed07-113">ป้อน**ชนิดของ DNS** : **CNAME (นามแฝง)**</span><span class="sxs-lookup"><span data-stu-id="bed07-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="bed07-114">สำหรับ**ชื่อโฮสต์หรือนามแฝง**พิมพ์ต่อไปนี้: **www**</span><span class="sxs-lookup"><span data-stu-id="bed07-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="bed07-115">สำหรับ**จุดที่อยู่**พิมพ์ชื่อโดเมน(แบบเต็ม FQDN) สำหรับเว็บไซต์ของคุณ (ตัวอย่างเช่น contoso.com)</span><span class="sxs-lookup"><span data-stu-id="bed07-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="bed07-116">เลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="bed07-116">Select **Save**.</span></span> 
    

