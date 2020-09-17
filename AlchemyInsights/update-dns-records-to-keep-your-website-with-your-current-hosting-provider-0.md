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
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815804"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="b602a-102">อัปเดตระเบียน DNS เพื่อเก็บเว็บไซต์ของคุณไว้กับผู้ให้บริการโฮสต์ปัจจุบันของคุณ</span><span class="sxs-lookup"><span data-stu-id="b602a-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="b602a-103">ในศูนย์การจัดการ Microsoft ๓๖๕ให้ไปที่หน้า**Setup**  >  [โดเมน](https://admin.microsoft.com/Adminportal#/Domains)การตั้งค่าและในรายการโดเมนให้เลือกโดเมนที่คุณกำลังใช้สำหรับเว็บไซต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="b602a-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="b602a-104">เลือก **+ ระเบียนแบบกำหนดเองใหม่** แล้วใส่ข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b602a-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="b602a-105">สำหรับ **ชนิด DNS** ให้ใส่: **A (ที่อยู่)**</span><span class="sxs-lookup"><span data-stu-id="b602a-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="b602a-106">สำหรับ **ชื่อโฮสต์หรือนามแฝง**ให้พิมพ์ดังต่อไปนี้: **@**</span><span class="sxs-lookup"><span data-stu-id="b602a-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="b602a-107">สำหรับ **ที่อยู่ ip**ให้พิมพ์ที่อยู่ ip แบบคงที่สำหรับเว็บไซต์ของคุณที่โฮสต์อยู่ในปัจจุบัน (ตัวอย่างเช่น 172.16.140.1)</span><span class="sxs-lookup"><span data-stu-id="b602a-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="b602a-108">การทำเช่นนี้จะต้องเป็นที่อยู่ ip แบบ*คง*ที่สำหรับเว็บไซต์ไม่ใช่ที่อยู่ ip*แบบไดนามิก*</span><span class="sxs-lookup"><span data-stu-id="b602a-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="b602a-109">ตรวจสอบกับไซต์ที่โฮสต์เว็บไซต์ของคุณเพื่อให้แน่ใจว่าคุณจะได้รับที่อยู่ IP แบบคงที่สำหรับเว็บไซต์สาธารณะของคุณ</span><span class="sxs-lookup"><span data-stu-id="b602a-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="b602a-110">เลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="b602a-110">Select **Save**.</span></span>

<span data-ttu-id="b602a-111">นอกจากนี้คุณยังสามารถสร้างระเบียน CNAME เพื่อช่วยให้ลูกค้าค้นหาเว็บไซต์ของคุณได้</span><span class="sxs-lookup"><span data-stu-id="b602a-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="b602a-112">เลือก **+ ระเบียนแบบกำหนดเองใหม่** แล้วใส่ข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b602a-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="b602a-113">สำหรับ **ชนิด DNS** ให้ใส่: **CNAME (นามแฝง)**</span><span class="sxs-lookup"><span data-stu-id="b602a-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="b602a-114">สำหรับ **ชื่อโฮสต์หรือนามแฝง**ให้พิมพ์ดังต่อไปนี้: **www**</span><span class="sxs-lookup"><span data-stu-id="b602a-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="b602a-115">สำหรับ **ที่อยู่ชี้ไปยัง**ให้พิมพ์ชื่อโดเมนแบบเต็ม (FQDN) สำหรับเว็บไซต์ของคุณ (ตัวอย่างเช่น contoso.com)</span><span class="sxs-lookup"><span data-stu-id="b602a-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="b602a-116">เลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="b602a-116">Select **Save**.</span></span>
