---
title: การเข้าถึงถูกปฏิเสธเมื่อแมปไดรฟ์ไปยัง SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 23ee86df5404b6f20f3a4b605038b31b6f9fd731
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687385"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="efc3c-102">แก้ไขปัญหาเกี่ยวกับไลบรารี SharePoint ที่แมปไปยังไดรฟ์เครือข่าย</span><span class="sxs-lookup"><span data-stu-id="efc3c-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="efc3c-103">เมื่อคุณเรียกดูไปยังไดรฟ์เครือข่ายที่แมป</span><span class="sxs-lookup"><span data-stu-id="efc3c-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="efc3c-104">**\\ไม่สามารถเข้าถึงเส้นทางได้ คุณอาจไม่มีสิทธิ์ในการใช้ทรัพยากรเครือข่ายนี้ ติดต่อผู้ดูแลเซิร์ฟเวอร์นี้เพื่อดูว่าคุณมีสิทธิ์ในการเข้าถึงหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="efc3c-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="efc3c-105">**การเข้าถึงถูกปฏิเสธ ก่อนที่จะเปิดแฟ้มในตําแหน่งนี้**</span><span class="sxs-lookup"><span data-stu-id="efc3c-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="efc3c-106">[รับความช่วยเหลือในการแก้ไขปัญหาเครือข่ายที่แมป](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)</span><span class="sxs-lookup"><span data-stu-id="efc3c-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="efc3c-107">การแมปไลบรารีเป็นไดรฟ์เครือข่ายชั่วคราว และสนับสนุนเฉพาะใน Internet Explorer เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="efc3c-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="efc3c-108">ซิงค์แฟ้ม[SharePoint กับไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx)ซึ่งรวมถึง[แฟ้มตามต้องการ](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)</span><span class="sxs-lookup"><span data-stu-id="efc3c-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="efc3c-109">เข้าถึงไฟล์ทั้งหมดของคุณใน OneDrive โดยไม่ต้องใช้พื้นที่จัดเก็บข้อมูลภายในเครื่อง</span><span class="sxs-lookup"><span data-stu-id="efc3c-109">Access all your files in OneDrive without using local storage space.</span></span>
  