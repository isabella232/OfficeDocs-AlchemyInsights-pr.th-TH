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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>แผนของช่วงที่อยู่ IP ขาออกของ EOP

เราตรวจพบปัญหาที่อาจเกิดขึ้นกับองค์กรของคุณที่ (ถ้าไม่ได้แก้ไขโดยวันที่26ตุลาคม๒๐๑๘) อาจแบ่งจดหมายเวียนไปยังปลายทางภายในองค์กรหรือภายนอกของคุณ เมื่อมีการสื่อสารก่อนหน้านี้เพื่อลดความซับซ้อนของการจัดการช่วงที่อยู่ IP เราจะรวมช่วงที่อยู่ IP Exchange Online Protection (EOP) ที่ใช้ในการส่งและรับอีเมลที่อยู่ภายนอก Microsoft ๓๖๕ การวิเคราะห์ของเราระบุว่าหนึ่งหรือหลายแหล่งอีเมลภายนอกที่คุณได้กำหนดค่าในตัวเชื่อมต่อโฟลว์จดหมายไม่ยอมรับการเชื่อมต่อจากช่วงที่อยู่ IP ที่แสดงไว้[ที่นี่](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

ดำเนินการก่อนวันที่26ตุลาคมเพื่อให้แน่ใจว่าแหล่งข้อมูลและจุดหมายเหล่านี้จะยอมรับการเชื่อมต่อและจาก [ที่อยู่ IP ที่เผยแพร่](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)แล้วทั้งหมดของ EOP

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเปลี่ยนแปลงนี้โปรดดูที่ประกาศศูนย์ข้อความ[MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)หรือ[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**หมายเหตุ**: ถ้าคุณเคยใช้การเผยแพร่ IP หรือ URL ผ่านทาง HTML, XML และ RSS สำหรับการอัปเดตจุดสิ้นสุดคุณควรโยกย้ายไปยังบริการเว็บใหม่สำหรับการทำให้การอัปเดตเหล่านี้อัตโนมัติ สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ประเภทจุดสิ้นสุดของ microsoft ๓๖๕และที่อยู่ IP ของ microsoft ๓๖๕และบริการเว็บ URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
