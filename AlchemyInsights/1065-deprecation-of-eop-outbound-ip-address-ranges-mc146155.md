---
title: 1065 deprecation ของ EOP ขาออก IP ที่อยู่ rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 2b4b2e2341f45e2d37713d72a2e0d34fa1a9a7cc
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934903"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="64696-102">Deprecation ของช่วงที่อยู่ IP ขาออก EOP</span><span class="sxs-lookup"><span data-stu-id="64696-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="64696-p101">เราได้ตรวจพบการตัดสินค้าจากคลังที่อาจเกิดขึ้นกับองค์กรของคุณที่ (ถ้าไม่ถูกแก้ไข โดย 26th ตุลาคม 2018) อาจใช้การรับส่งจดหมายของคุณในสถานที่หรือปลายทางภายนอก เป็นก่อนหน้านี้สื่อสารกับ เพื่อให้จัดการช่วงที่อยู่ IP เราจะรวมช่วงอยู่ IP ป้องกันแบบออนไลน์ของอัตราแลกเปลี่ยน (EOP) ที่ใช้ในการส่ง และรับอีเมลภายนอก Office 365 การวิเคราะห์ของเราบ่งชี้ว่า หนึ่งหรือหลายแหล่งภายนอกอีเมลหรือปลายทางที่คุณได้กำหนดค่าให้เป็นตัวเชื่อมต่อกระแสจดหมายไม่ยอมรับการเชื่อมต่อจาก IP อยู่ช่วงแสดงอยู่[ที่นี่](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)</span><span class="sxs-lookup"><span data-stu-id="64696-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="64696-106">ดำเนินการก่อนเดือน 26th ตุลาคมเพื่อให้แน่ใจว่า แหล่งที่มาและปลายทางเหล่านี้จะยอมรับการเชื่อมต่อไปยัง และจากทั้งหมด[เผยแพร่ EOP IP แอดเดรส](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)</span><span class="sxs-lookup"><span data-stu-id="64696-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="64696-107">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเปลี่ยนแปลงนี้ โปรดดูศูนย์ข้อความประกาศ[MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)หรือ[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)</span><span class="sxs-lookup"><span data-stu-id="64696-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="64696-p102">**หมายเหตุ**: ถ้าคุณใช้มาก่อนประกาศ IP หรือ URL ผ่าน HTML, XML และ RSS สำหรับปลายทางในการปรับปรุง คุณยังควรโยกย้ายไปยังเว็บเซอร์ใหม่สำหรับการทำงานอัตโนมัติสำหรับการปรับปรุงชนิดนี้ สำหรับข้อมูลเพิ่มเติม ดู[ประเภทปลายทาง Office 365 และที่อยู่ IP ของ Office 365 และบริการเว็บ URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)</span><span class="sxs-lookup"><span data-stu-id="64696-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

