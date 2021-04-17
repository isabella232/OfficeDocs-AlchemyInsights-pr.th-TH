---
title: อัปเดตระเบียน DNS เพื่อเก็บเว็บไซต์ของคุณกับผู้ให้บริการโฮสต์ปัจจุบันของคุณ
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827558"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="e64e5-102">อัปเดตระเบียน DNS เพื่อเก็บเว็บไซต์ของคุณกับผู้ให้บริการโฮสต์ปัจจุบันของคุณ</span><span class="sxs-lookup"><span data-stu-id="e64e5-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="e64e5-103">ในศูนย์การจัดการ Microsoft 365 ให้ไปที่หน้าตั้งค่าโดเมน และในรายการโดเมน  >  [](https://admin.microsoft.com/Adminportal#/Domains)ให้เลือกโดเมนที่คุณใช้กับเว็บไซต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="e64e5-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="e64e5-104">เลือก **+ ระเบียนแบบปรับแต่งเอง** ใหม่ แล้วใส่ข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e64e5-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="e64e5-105">For **DNS type** enter: A **(Address)**</span><span class="sxs-lookup"><span data-stu-id="e64e5-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="e64e5-106">For **Host name or Alias**, type the following: **@**</span><span class="sxs-lookup"><span data-stu-id="e64e5-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="e64e5-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="e64e5-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="e64e5-108">ซึ่ง  *ต้องเป็นที่อยู่*  IP แบบคงที่ของเว็บไซต์ ไม่ใช่  *ที่อยู่*  IP แบบไดนามิก</span><span class="sxs-lookup"><span data-stu-id="e64e5-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="e64e5-109">ตรวจสอบกับไซต์ที่เว็บไซต์ของคุณถูกโฮสต์เพื่อให้แน่ใจว่าคุณสามารถรับที่อยู่ IP แบบคงที่ของเว็บไซต์สาธารณะของคุณ</span><span class="sxs-lookup"><span data-stu-id="e64e5-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="e64e5-110">เลือกบันทึก</span><span class="sxs-lookup"><span data-stu-id="e64e5-110">Select **Save**.</span></span>

<span data-ttu-id="e64e5-111">นอกจากนี้ คุณสามารถสร้างระเบียน CNAME เพื่อช่วยให้ลูกค้าค้นหาเว็บไซต์ของคุณได้</span><span class="sxs-lookup"><span data-stu-id="e64e5-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="e64e5-112">เลือก **+ ระเบียนแบบปรับแต่งเอง** ใหม่ แล้วใส่ข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e64e5-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="e64e5-113">For **DNS type** enter: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="e64e5-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="e64e5-114">For **Host name or Alias**, type the following: **www**</span><span class="sxs-lookup"><span data-stu-id="e64e5-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="e64e5-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="e64e5-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="e64e5-116">เลือกบันทึก</span><span class="sxs-lookup"><span data-stu-id="e64e5-116">Select **Save**.</span></span>
