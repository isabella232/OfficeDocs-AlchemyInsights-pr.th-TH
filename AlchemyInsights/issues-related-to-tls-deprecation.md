---
title: ไม่สามารถส่ง/รับอีเมลไปยัง/จาก Office 365 ได้เนื่องจากปิดใช้งาน TLS 1.0 และ TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747114"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>ไม่สามารถส่ง/รับอีเมลไปยัง/จาก Office 365 ได้เนื่องจากปิดใช้งาน TLS 1.0 และ TLS 1.1

ตามที่ยืนยันโดยศูนย์ข้อความโพสต์ MC229914, TLS 1.0 และ deprecation TLS 1.1 เริ่มบังคับใช้จุดสิ้นสุดการโฟลว์จดหมาย Exchange Online Office 365 จะไม่ยอมรับการเชื่อมต่ออีเมล TLS 1.0 และ TLS 1.1 จากแหล่งข้อมูลภายนอกอีกต่อไป นอกจากนี้ Exchange Online จะไม่ใช้ TLS 1.0 หรือ 1.1 เพื่อส่งอีเมลขาออก ถ้าคุณพบปัญหาเนื่องจากปิดใช้งาน TLS 1.0 หรือ 1.1 คุณอาจพบหนึ่งในข้อผิดพลาดต่อไปนี้

- ผู้ส่งได้รับ NDR เด้งกลับมา - การเชื่อมต่อ '421 4.4.2 ลดลงเนื่องจาก SocketError'
- ข้อผิดพลาดในตัวแสดงคิวของเซิร์ฟเวอร์ภายในองค์กรที่ส่งอีเมลถึง Officer 365- '421 4.4.2 การเชื่อมต่อลดลงเนื่องจาก SocketError'
- ข้อผิดพลาดในบันทึก [Send](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) connector Protocol บนเซิร์ฟเวอร์ที่ส่งอีเมลไปยัง Office 365- การตกลงเกี่ยวกับ TLS ล้มเหลวด้วยข้อผิดพลาด SocketError
- ข้อผิดพลาดในการส่งหรือรับบันทึกโพรโทคอลตัวเชื่อมต่อ - '451 5.7.3 ต้องออกสั่ง STARTTLS ก่อน'

ถ้าคุณพบข้อผิดพลาดข้างต้นโปรดตรวจสอบให้แน่ใจว่าเซิร์ฟเวอร์ที่ส่งหรือรับอีเมลมีการเปิดใช้งาน TLS 1.2 โดยการตรวจสอบรีจิสทรีคีย์ต่อไปนี้-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

ถ้าคุณเปลี่ยนแปลงรีจิสทรีคีย์ข้างต้นเพื่อเปิดใช้งาน TLS 1.2 ให้รีสตาร์ตเซิร์ฟเวอร์เพื่อให้การเปลี่ยนแปลงมีผล นอกจากนี้ ตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งการอัปเดต Windows และ Exchange เวอร์ชันล่าสุดแล้ว

สำหรับข้อมูลเพิ่มเติม ให้ดูที่

- [Exchange Server TLS guidance, part 1: เตรียมพร้อมสําหรับ TLS 1.2 - ชุมชนด้านเทคนิคของ Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS guidance Part 2: การเปิดใช้งาน TLS 1.2 และการระบุไคลเอ็นต์ที่ไม่ได้ใช้ - ชุมชนด้านเทคนิคของ Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [การความเข้าใจสถานการณ์อีเมลถ้าเวอร์ชัน TLS ไม่สามารถยอมรับกับ Exchange Online - ชุมชนด้านเทคนิคของ Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
