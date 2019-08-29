---
title: อัปเดตระเบียน DNS เพื่อให้เว็บไซต์ของคุณมีผู้ให้บริการโฮสติ้งปัจจุบันของคุณ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665779"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="4a108-102">อัปเดตระเบียน DNS เพื่อให้เว็บไซต์ของคุณมีผู้ให้บริการโฮสติ้งปัจจุบันของคุณ</span><span class="sxs-lookup"><span data-stu-id="4a108-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="4a108-103">ในศูนย์กลางการดูแลระบบ Microsoft ๓๖๕ไปที่หน้า[โดเมน](https://portal.office.com/adminportal/home#/Domains)**การตั้งค่า** > และในรายการโดเมนให้เลือกโดเมนที่คุณใช้สำหรับเว็บไซต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="4a108-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="4a108-104">เลือก **+ ระเบียนที่กำหนดเองใหม่**และป้อนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="4a108-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="4a108-105">สำหรับ**ชนิด DNS**ป้อน: **A (ที่อยู่)**</span><span class="sxs-lookup"><span data-stu-id="4a108-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="4a108-106">สำหรับ**ชื่อโฮสต์หรือ Alias**ให้พิมพ์ดังต่อไปนี้:**@**</span><span class="sxs-lookup"><span data-stu-id="4a108-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="4a108-107">สำหรับ**ที่อยู่ ip**ให้พิมพ์ที่อยู่ ip แบบคงที่สำหรับเว็บไซต์ของคุณที่เป็นโฮสต์ในปัจจุบัน (ตัวอย่างเช่น 172.16.140.1)</span><span class="sxs-lookup"><span data-stu-id="4a108-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="4a108-108">ซึ่งจะต้องเป็นที่อยู่ ip แบบ*คง*ที่สำหรับเว็บไซต์ไม่ใช่ที่อยู่ ip*ไดนามิก*</span><span class="sxs-lookup"><span data-stu-id="4a108-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="4a108-109">ตรวจสอบกับเว็บไซต์ที่โฮสต์เว็บไซต์ของคุณเพื่อให้แน่ใจว่าคุณจะได้รับที่อยู่ IP แบบคงที่สำหรับเว็บไซต์สาธารณะของคุณ</span><span class="sxs-lookup"><span data-stu-id="4a108-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="4a108-110">เลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="4a108-110">Select **Save**.</span></span>

<span data-ttu-id="4a108-111">นอกจากนี้คุณสามารถสร้างระเบียน CNAME เพื่อช่วยให้ลูกค้าพบเว็บไซต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="4a108-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="4a108-112">เลือก **+ ระเบียนที่กำหนดเองใหม่**และป้อนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="4a108-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="4a108-113">สำหรับ**ประเภท DNS**ป้อน: **CNAME (นามแฝง)**</span><span class="sxs-lookup"><span data-stu-id="4a108-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="4a108-114">สำหรับ**ชื่อโฮสต์หรือ Alias**ให้พิมพ์ดังต่อไปนี้: **www**</span><span class="sxs-lookup"><span data-stu-id="4a108-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="4a108-115">สำหรับ**จุดที่อยู่**ให้พิมพ์ชื่อโดเมน (แบบเต็ม FQDN) สำหรับเว็บไซต์ของคุณ (ตัวอย่างเช่น contoso.com)</span><span class="sxs-lookup"><span data-stu-id="4a108-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="4a108-116">เลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="4a108-116">Select **Save**.</span></span>
