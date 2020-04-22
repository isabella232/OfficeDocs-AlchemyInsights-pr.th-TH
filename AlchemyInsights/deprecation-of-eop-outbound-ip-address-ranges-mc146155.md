---
title: การเสื่อมสภาพ 1065 ของช่วงที่อยู่ IP ขาออกของ EOPMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704616"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="5fc0c-102">การเสื่อมสภาพของช่วงที่อยู่ IP ขาออกของ EOP</span><span class="sxs-lookup"><span data-stu-id="5fc0c-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="5fc0c-103">เราได้ตรวจพบปัญหาที่อาจเกิดขึ้นกับองค์กรของคุณซึ่ง (หากไม่ได้รับการแก้ไขภายในวันที่ 26 ตุลาคม 2018) อาจแบ่งลําดับจดหมายไปยังปลายทางในสถานที่หรือปลายทางภายนอกของคุณ</span><span class="sxs-lookup"><span data-stu-id="5fc0c-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="5fc0c-104">ดังที่ได้กล่าวมาก่อนหน้านี้ว่า เพื่อให้การจัดการช่วงที่อยู่ IP ง่ายขึ้น</span><span class="sxs-lookup"><span data-stu-id="5fc0c-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="5fc0c-105">การวิเคราะห์ของเราบ่งชี้ว่าอย่างน้อยหนึ่งแหล่งที่มาของอีเมลภายนอกหรือปลายทางที่คุณได้กําหนดค่าในตัวเชื่อมต่อกระแสจดหมายไม่ยอมรับการเชื่อมต่อจากช่วงที่อยู่ IP ที่แสดง[ที่นี่](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)</span><span class="sxs-lookup"><span data-stu-id="5fc0c-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="5fc0c-106">กระทําก่อนวันที่ 26 ตุลาคมเพื่อให้แน่ใจว่าแหล่งข้อมูลและปลายทางเหล่านี้จะยอมรับการเชื่อมต่อและจาก[ที่อยู่ IP EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)ที่เผยแพร่ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="5fc0c-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="5fc0c-107">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการเปลี่ยนแปลงนี้ โปรดดู ข้อความศูนย์ข้อความติด[ประกาศ MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)หรือ[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)</span><span class="sxs-lookup"><span data-stu-id="5fc0c-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="5fc0c-108">**หมายเหตุ**: ถ้าคุณเคยใช้การเผยแพร่ IP หรือ URL ผ่านทาง HTML, XML และ RSS สําหรับการปรับปรุงปลายทาง คุณควรย้ายไปยังบริการเว็บใหม่สําหรับการปรับปรุงประเภทนี้โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="5fc0c-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="5fc0c-109">สําหรับข้อมูลเพิ่มเติม โปรดดูที่[ประเภทปลายทางของ Microsoft 365 และที่อยู่ IP ของ Microsoft 365 และบริการเว็บ URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)</span><span class="sxs-lookup"><span data-stu-id="5fc0c-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
