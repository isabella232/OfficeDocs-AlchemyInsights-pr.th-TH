---
title: การเข้าถึงถูกปฏิเสธเมื่อแมปไดรฟ์ไปยัง SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668762"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="049a9-102">แก้ไขปัญหาเกี่ยวกับไลบรารี SharePoint ที่แมปไปยังไดรฟ์เครือข่าย</span><span class="sxs-lookup"><span data-stu-id="049a9-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="049a9-103">เมื่อคุณเรียกดูไปยังไดรฟ์เครือข่ายที่แมปคุณอาจเห็นหนึ่งในข้อความต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="049a9-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="049a9-104">**\\ไม่สามารถเข้าถึงเส้นทางได้ คุณอาจไม่มีสิทธิ์ในการใช้ทรัพยากรเครือข่ายนี้ ติดต่อผู้ดูแลเซิร์ฟเวอร์นี้เพื่อค้นหาว่าคุณมีสิทธิ์ในการเข้าถึงหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="049a9-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="049a9-105">**การเข้าถึงถูกปฏิเสธ ก่อนที่จะเปิดไฟล์ในตำแหน่งที่ตั้งนี้ก่อนอื่นคุณต้องเพิ่มเว็บไซต์ลงในรายการไซต์ที่เชื่อถือได้ของคุณจากนั้นเรียกดูเว็บไซต์และเลือกตัวเลือกเพื่อเข้าสู่ระบบโดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="049a9-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="049a9-106">[รับความช่วยเหลือในการแก้ไขปัญหาการแมปไดรฟ์เครือข่าย](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)</span><span class="sxs-lookup"><span data-stu-id="049a9-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="049a9-107">การแมปไลบรารีเป็นไดรฟ์เครือข่ายเป็นการชั่วคราวและได้รับการสนับสนุนใน Internet Explorer เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="049a9-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="049a9-108">แทนที่ [ซิงค์ไฟล์ SharePoint ด้วยไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) ที่รวม [ไฟล์ตามความต้อง](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)การ</span><span class="sxs-lookup"><span data-stu-id="049a9-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="049a9-109">เข้าถึงไฟล์ทั้งหมดของคุณใน OneDrive ได้โดยไม่ต้องใช้พื้นที่เก็บข้อมูลภายในเครื่อง</span><span class="sxs-lookup"><span data-stu-id="049a9-109">Access all your files in OneDrive without using local storage space.</span></span>
  