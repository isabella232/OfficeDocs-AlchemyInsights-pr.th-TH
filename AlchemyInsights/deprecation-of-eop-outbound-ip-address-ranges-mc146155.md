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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>การเสื่อมสภาพของช่วงที่อยู่ IP ขาออกของ EOP

เราได้ตรวจพบปัญหาที่อาจเกิดขึ้นกับองค์กรของคุณซึ่ง (หากไม่ได้รับการแก้ไขภายในวันที่ 26 ตุลาคม 2018) อาจแบ่งลําดับจดหมายไปยังปลายทางในสถานที่หรือปลายทางภายนอกของคุณ ดังที่ได้กล่าวมาก่อนหน้านี้ว่า เพื่อให้การจัดการช่วงที่อยู่ IP ง่ายขึ้น การวิเคราะห์ของเราบ่งชี้ว่าอย่างน้อยหนึ่งแหล่งที่มาของอีเมลภายนอกหรือปลายทางที่คุณได้กําหนดค่าในตัวเชื่อมต่อกระแสจดหมายไม่ยอมรับการเชื่อมต่อจากช่วงที่อยู่ IP ที่แสดง[ที่นี่](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

กระทําก่อนวันที่ 26 ตุลาคมเพื่อให้แน่ใจว่าแหล่งข้อมูลและปลายทางเหล่านี้จะยอมรับการเชื่อมต่อและจาก[ที่อยู่ IP EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)ที่เผยแพร่ทั้งหมด

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการเปลี่ยนแปลงนี้ โปรดดู ข้อความศูนย์ข้อความติด[ประกาศ MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)หรือ[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**หมายเหตุ**: ถ้าคุณเคยใช้การเผยแพร่ IP หรือ URL ผ่านทาง HTML, XML และ RSS สําหรับการปรับปรุงปลายทาง คุณควรย้ายไปยังบริการเว็บใหม่สําหรับการปรับปรุงประเภทนี้โดยอัตโนมัติ สําหรับข้อมูลเพิ่มเติม โปรดดูที่[ประเภทปลายทางของ Microsoft 365 และที่อยู่ IP ของ Microsoft 365 และบริการเว็บ URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
