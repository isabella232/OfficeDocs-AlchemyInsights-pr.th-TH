---
title: การเข้าถึงถูกปฏิเสธเมื่อคุณแมปไดรฟ์ไปยัง SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: d6896e9c2b2b4b428459b4c0f3aee0658b02322e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927811"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="7b1c1-102">แก้ไขปัญหาเกี่ยวกับไลบรารี SharePoint ที่แมปไปยังไดรฟ์เครือข่าย</span><span class="sxs-lookup"><span data-stu-id="7b1c1-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="7b1c1-103">เมื่อคุณเรียกดูไปยังไดรฟ์เครือข่ายที่แมป คุณอาจเห็นข้อความแสดงข้อต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7b1c1-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="7b1c1-104">**\\เส้นทางไม่สามารถเข้าถึงได้ คุณอาจไม่มีสิทธิ์ในการใช้ทรัพยากรเครือข่ายนี้ ติดต่อผู้ดูแลระบบเซิร์ฟเวอร์นี้เพื่อค้นหาถ้าคุณมีสิทธิ์การเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="7b1c1-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>
    
- <span data-ttu-id="7b1c1-105">**การเข้าถึงถูกปฏิเสธ ก่อนที่จะเปิดแฟ้มในตำแหน่งนี้ คุณต้องก่อนเพิ่มเว็บไซต์ลงในรายการไซต์ที่เชื่อถือได้ของคุณ เรียกดูไปยังเว็บไซต์ และเลือกตัวเลือกเพื่อเข้าสู่ระบบโดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="7b1c1-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>
    
<span data-ttu-id="7b1c1-106">[แก้ปัญหาวิธีการรับการแมปไดรฟ์เครือข่าย](https://support.office.com/article/ef399c67-4578-4c3a-adbe-0b489084eabe.aspx)</span><span class="sxs-lookup"><span data-stu-id="7b1c1-106">[Get help troubleshooting mapped network drives](https://support.office.com/article/ef399c67-4578-4c3a-adbe-0b489084eabe.aspx).</span></span>
  
<span data-ttu-id="7b1c1-p101">ไลบรารีเป็นไดรฟ์เครือข่ายที่แมปเป็นแบบชั่วคราว และได้รับการสนับสนุนเฉพาะใน Internet Explorer แทน[ซิงค์แฟ้ม SharePoint ด้วยไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx)ซึ่งรวมถึง[แฟ้มตามความต้องการ](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx) เข้าถึงแฟ้มของคุณทั้งหมดใน OneDrive โดยไม่ต้องใช้เนื้อที่เก็บข้อมูลภายในเครื่อง</span><span class="sxs-lookup"><span data-stu-id="7b1c1-p101">Mapping a library as a network drive is temporary and supported only in Internet Explorer. Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx). Access all your files in OneDrive without using local storage space.</span></span>
  

