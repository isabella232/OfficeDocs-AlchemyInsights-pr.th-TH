---
title: การเลิกใช้ 1065 ของช่วงที่อยู่ IP ขาออกของ EOPMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031281"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>การเลิกใช้ช่วงที่อยู่ IP ขาออกของ EOP

เราตรวจพบปัญหาที่อาจเกิดขึ้นกับองค์กรของคุณว่า (ถ้าไม่ได้แก้ไขภายในวันที่ 26 ตุลาคม 2018) อาจตัดการส่งจดหมายไปยังปลายทางภายในองค์กรของคุณหรือปลายทางภายนอก ดังที่กล่าวมาก่อนหน้านี้ เมื่อต้องการลดความซับซ้อนในการจัดการช่วงที่อยู่ IP เรารวมช่วงที่อยู่ IP Exchange Online Protection (EOP) ที่ใช้ในการส่งและรับอีเมลภายนอกMicrosoft 365 การวิเคราะห์ของเราระบุว่า อย่างน้อยหนึ่งแหล่งอีเมลภายนอกหรือปลายทางที่คุณกําหนดค่าในตัวเชื่อมต่อลโฟลว์จดหมายไม่ยอมรับการเชื่อมต่อจากช่วงที่อยู่ IP [ที่แสดง](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)ไว้ที่นี่

ปฏิบัติตามก่อนวันที่ 26 ตุลาคมเพื่อให้แน่ใจว่าแหล่งข้อมูลและปลายทางเหล่านี้จะยอมรับการเชื่อมต่อและจากที่อยู่ [IP EOP ที่เผยแพร่](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)ทั้งหมด

For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**หมายเหตุ**: ถ้าคุณเคยใช้การเผยแพร่ IP หรือ URL ผ่าน HTML, XML และ RSS เพื่ออัปเดตจุดสิ้นสุด คุณควรโยกย้ายไปยังบริการเว็บใหม่เพื่ออัตโนมัติชนิดของการอัปเดตเหล่านี้ For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
