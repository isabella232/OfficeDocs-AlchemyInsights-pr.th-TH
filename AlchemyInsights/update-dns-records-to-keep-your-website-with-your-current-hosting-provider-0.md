---
title: อัปเดตระเบียน DNS เพื่อเก็บเว็บไซต์ของคุณไว้กับผู้ให้บริการโฮสต์ปัจจุบันของคุณ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 2f2d4f7c093d62267bb859e96493ec6d09452c7e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699538"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="e51e2-102">อัปเดตระเบียน DNS เพื่อเก็บเว็บไซต์ของคุณไว้กับผู้ให้บริการโฮสต์ปัจจุบันของคุณ</span><span class="sxs-lookup"><span data-stu-id="e51e2-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="e51e2-103">ในศูนย์การจัดการ Microsoft ๓๖๕ให้ไปที่หน้า**Setup**  >  [โดเมน](https://portal.office.com/adminportal/home#/Domains)การตั้งค่าและในรายการโดเมนให้เลือกโดเมนที่คุณกำลังใช้สำหรับเว็บไซต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="e51e2-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="e51e2-104">เลือก **+ ระเบียนแบบกำหนดเองใหม่** แล้วใส่ข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e51e2-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="e51e2-105">สำหรับ **ชนิด DNS** ให้ใส่: **A (ที่อยู่)**</span><span class="sxs-lookup"><span data-stu-id="e51e2-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="e51e2-106">สำหรับ **ชื่อโฮสต์หรือนามแฝง**ให้พิมพ์ดังต่อไปนี้: **@**</span><span class="sxs-lookup"><span data-stu-id="e51e2-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="e51e2-107">สำหรับ **ที่อยู่ ip**ให้พิมพ์ที่อยู่ ip แบบคงที่สำหรับเว็บไซต์ของคุณที่โฮสต์อยู่ในปัจจุบัน (ตัวอย่างเช่น 172.16.140.1)</span><span class="sxs-lookup"><span data-stu-id="e51e2-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="e51e2-108">การทำเช่นนี้จะต้องเป็นที่อยู่ ip แบบ*คง*ที่สำหรับเว็บไซต์ไม่ใช่ที่อยู่ ip*แบบไดนามิก*</span><span class="sxs-lookup"><span data-stu-id="e51e2-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="e51e2-109">ตรวจสอบกับไซต์ที่โฮสต์เว็บไซต์ของคุณเพื่อให้แน่ใจว่าคุณจะได้รับที่อยู่ IP แบบคงที่สำหรับเว็บไซต์สาธารณะของคุณ</span><span class="sxs-lookup"><span data-stu-id="e51e2-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="e51e2-110">เลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="e51e2-110">Select **Save**.</span></span>

<span data-ttu-id="e51e2-111">นอกจากนี้คุณยังสามารถสร้างระเบียน CNAME เพื่อช่วยให้ลูกค้าค้นหาเว็บไซต์ของคุณได้</span><span class="sxs-lookup"><span data-stu-id="e51e2-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="e51e2-112">เลือก **+ ระเบียนแบบกำหนดเองใหม่** แล้วใส่ข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e51e2-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="e51e2-113">สำหรับ **ชนิด DNS** ให้ใส่: **CNAME (นามแฝง)**</span><span class="sxs-lookup"><span data-stu-id="e51e2-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="e51e2-114">สำหรับ **ชื่อโฮสต์หรือนามแฝง**ให้พิมพ์ดังต่อไปนี้: **www**</span><span class="sxs-lookup"><span data-stu-id="e51e2-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="e51e2-115">สำหรับ **ที่อยู่ชี้ไปยัง**ให้พิมพ์ชื่อโดเมนแบบเต็ม (FQDN) สำหรับเว็บไซต์ของคุณ (ตัวอย่างเช่น contoso.com)</span><span class="sxs-lookup"><span data-stu-id="e51e2-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="e51e2-116">เลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="e51e2-116">Select **Save**.</span></span>
