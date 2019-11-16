---
title: การเข้าถึงถูกปฏิเสธเมื่อทำการแมปไดรฟ์ไปยัง SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/15/2019
ms.locfileid: "36737496"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="0345d-102">แก้ไขปัญหาเกี่ยวกับไลบรารี SharePoint ที่ถูกแมปไปยังไดรฟ์เครือข่าย</span><span class="sxs-lookup"><span data-stu-id="0345d-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="0345d-103">เมื่อคุณเรียกดูไปยังไดรฟ์เครือข่ายที่แมปคุณอาจเห็นหนึ่งในข้อความต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0345d-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="0345d-104">**\\เส้นทางไม่สามารถเข้าถึงได้ คุณอาจไม่มีสิทธิ์ในการใช้ทรัพยากรเครือข่ายนี้ ติดต่อผู้ดูแลของเซิร์ฟเวอร์นี้เพื่อดูว่าคุณมีสิทธิ์การเข้าถึงหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="0345d-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="0345d-105">**ปฏิเสธการเข้าถึง ก่อนที่จะเปิดแฟ้มในตำแหน่งนี้คุณต้องเพิ่มเว็บไซต์ลงในรายการไซต์ที่เชื่อถือได้ของคุณก่อนเรียกดูเว็บไซต์และเลือกตัวเลือกเพื่อเข้าสู่ระบบโดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="0345d-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="0345d-106">[รับความช่วยเหลือในการแก้ปัญหาไดรฟ์เครือข่ายที่แมป](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)ไว้</span><span class="sxs-lookup"><span data-stu-id="0345d-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="0345d-107">การแมปไลบรารีเป็นไดรฟ์เครือข่ายเป็นแบบถาวรและได้รับการสนับสนุนใน Internet Explorer เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="0345d-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="0345d-108">ให้[ซิงค์แฟ้ม SharePoint กับไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx)ซึ่งมี[แฟ้มตามความต้อง](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)การแทน</span><span class="sxs-lookup"><span data-stu-id="0345d-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="0345d-109">เข้าถึงไฟล์ทั้งหมดของคุณใน OneDrive โดยไม่ต้องใช้พื้นที่จัดเก็บข้อมูลภายใน</span><span class="sxs-lookup"><span data-stu-id="0345d-109">Access all your files in OneDrive without using local storage space.</span></span>
  