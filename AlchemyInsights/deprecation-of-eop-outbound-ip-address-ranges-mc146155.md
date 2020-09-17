---
title: ๑๐๖๕แผนของ EOP ที่อยู่ IP ขาออก rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806814"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="e74e3-102">แผนของช่วงที่อยู่ IP ขาออกของ EOP</span><span class="sxs-lookup"><span data-stu-id="e74e3-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="e74e3-103">เราตรวจพบปัญหาที่อาจเกิดขึ้นกับองค์กรของคุณที่ (ถ้าไม่ได้แก้ไขโดยวันที่26ตุลาคม๒๐๑๘) อาจแบ่งจดหมายเวียนไปยังปลายทางภายในองค์กรหรือภายนอกของคุณ</span><span class="sxs-lookup"><span data-stu-id="e74e3-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="e74e3-104">เมื่อมีการสื่อสารก่อนหน้านี้เพื่อลดความซับซ้อนของการจัดการช่วงที่อยู่ IP เราจะรวมช่วงที่อยู่ IP Exchange Online Protection (EOP) ที่ใช้ในการส่งและรับอีเมลที่อยู่ภายนอก Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="e74e3-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="e74e3-105">การวิเคราะห์ของเราระบุว่าหนึ่งหรือหลายแหล่งอีเมลภายนอกที่คุณได้กำหนดค่าในตัวเชื่อมต่อโฟลว์จดหมายไม่ยอมรับการเชื่อมต่อจากช่วงที่อยู่ IP ที่แสดงไว้[ที่นี่](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)</span><span class="sxs-lookup"><span data-stu-id="e74e3-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="e74e3-106">ดำเนินการก่อนวันที่26ตุลาคมเพื่อให้แน่ใจว่าแหล่งข้อมูลและจุดหมายเหล่านี้จะยอมรับการเชื่อมต่อและจาก [ที่อยู่ IP ที่เผยแพร่](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)แล้วทั้งหมดของ EOP</span><span class="sxs-lookup"><span data-stu-id="e74e3-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="e74e3-107">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเปลี่ยนแปลงนี้โปรดดูที่ประกาศศูนย์ข้อความ[MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)หรือ[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)</span><span class="sxs-lookup"><span data-stu-id="e74e3-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="e74e3-108">**หมายเหตุ**: ถ้าคุณเคยใช้การเผยแพร่ IP หรือ URL ผ่านทาง HTML, XML และ RSS สำหรับการอัปเดตจุดสิ้นสุดคุณควรโยกย้ายไปยังบริการเว็บใหม่สำหรับการทำให้การอัปเดตเหล่านี้อัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="e74e3-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="e74e3-109">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ประเภทจุดสิ้นสุดของ microsoft ๓๖๕และที่อยู่ IP ของ microsoft ๓๖๕และบริการเว็บ URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)</span><span class="sxs-lookup"><span data-stu-id="e74e3-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
