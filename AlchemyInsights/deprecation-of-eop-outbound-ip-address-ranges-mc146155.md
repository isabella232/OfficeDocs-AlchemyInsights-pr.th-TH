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
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858115"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecation ของช่วงที่อยู่ IP ขาออก EOP

เราได้ตรวจพบการตัดสินค้าจากคลังที่อาจเกิดขึ้นกับองค์กรของคุณที่ (ถ้าไม่ถูกแก้ไข โดย 26th ตุลาคม 2018) อาจใช้การรับส่งจดหมายของคุณในสถานที่หรือปลายทางภายนอก เป็นก่อนหน้านี้สื่อสารกับ เพื่อให้จัดการช่วงที่อยู่ IP เราจะรวมช่วงอยู่ IP ป้องกันแบบออนไลน์ของอัตราแลกเปลี่ยน (EOP) ที่ใช้ในการส่ง และรับอีเมลภายนอก Office 365 การวิเคราะห์ของเราบ่งชี้ว่า หนึ่งหรือหลายแหล่งภายนอกอีเมลหรือปลายทางที่คุณได้กำหนดค่าให้เป็นตัวเชื่อมต่อกระแสจดหมายไม่ยอมรับการเชื่อมต่อจาก IP อยู่ช่วงแสดงอยู่[ที่นี่](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

ดำเนินการก่อนเดือน 26th ตุลาคมเพื่อให้แน่ใจว่า แหล่งที่มาและปลายทางเหล่านี้จะยอมรับการเชื่อมต่อไปยัง และจากทั้งหมด[เผยแพร่ EOP IP แอดเดรส](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเปลี่ยนแปลงนี้ โปรดดูศูนย์ข้อความประกาศ[MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)หรือ[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**หมายเหตุ**: ถ้าคุณใช้มาก่อนประกาศ IP หรือ URL ผ่าน HTML, XML และ RSS สำหรับปลายทางในการปรับปรุง คุณยังควรโยกย้ายไปยังเว็บเซอร์ใหม่สำหรับการทำงานอัตโนมัติสำหรับการปรับปรุงชนิดนี้ สำหรับข้อมูลเพิ่มเติม ดู[ประเภทปลายทาง Office 365 และที่อยู่ IP ของ Office 365 และบริการเว็บ URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
