---
title: ไม่สามารถส่ง/รับอีเมลไปยัง/จากOffice 365ปิดใช้งาน TLS 1.0 และ TLS 1.1
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054925"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>ไม่สามารถส่ง/รับอีเมลไปยัง/จากOffice 365ปิดใช้งาน TLS 1.0 และ TLS 1.1

ตามที่ยืนยันโดยโพสต์ศูนย์ข้อความ MC229914, TLS 1.0 และการเลิกใช้ TLS 1.1 เริ่มต้นบังคับใช้จุดสิ้นสุดลExchange OnlineลExchange Onlineลได้ ในOffice 365จะไม่ยอมรับการเชื่อมต่ออีเมล TLS 1.0 และ TLS 1.1 จากแหล่งข้อมูลภายนอกอีกต่อไป นอกจากนี้ Exchange Onlineจะไม่ใช้ TLS 1.0 หรือ 1.1 เพื่อส่งอีเมลขาออก ถ้าคุณพบปัญหาเนื่องจากปิดใช้งาน TLS 1.0 หรือ 1.1 คุณอาจพบหนึ่งในข้อผิดพลาดต่อไปนี้-

- ผู้ส่งได้รับ NDR ตีกลับ - '421 4.4.2 การเชื่อมต่อลดลงเนื่องจาก SocketError'
- ข้อผิดพลาดในตัวแสดงคิวของเซิร์ฟเวอร์ภายในองค์กรที่ส่งอีเมลถึง Officer 365- '421 4.4.2 การเชื่อมต่อลดลงเนื่องจาก SocketError'
- ข้อผิดพลาดใน ส่ง[บันทึกโพรโทคอลตัวเชื่อมต่อ](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging)บนเซิร์ฟเวอร์ที่ส่งอีเมลไปยังOffice 365- การOffice 365 TLS ล้มเหลวด้วยข้อผิดพลาด SocketError
- ข้อผิดพลาดใน ส่งหรือรับบันทึกโพรโทคอลตัวเชื่อมต่อ - '451 5.7.3 ต้องออกสั่ง STARTTLS ก่อน'

ถ้าคุณพบข้อผิดพลาดข้างต้น โปรดตรวจสอบให้แน่ใจว่าเซิร์ฟเวอร์ที่ส่งหรือรับอีเมลมีการเปิดใช้งาน TLS 1.2 โดยการตรวจสอบรีจิสทรีคีย์ต่อไปนี้-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

ถ้าคุณเปลี่ยนแปลงใดๆ ในรีจิสทรีคีย์ข้างต้นเพื่อเปิดใช้งาน TLS 1.2 ให้รีสตาร์ตเซิร์ฟเวอร์เพื่อให้การเปลี่ยนแปลงมีผล นอกจากนี้ ตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งการWindowsและExchangeล่าสุดแล้ว

สำหรับข้อมูลเพิ่มเติม ให้ดู:

- [Exchange Server แนวทาง TLS ส่วนที่ 1: เตรียมพร้อมสําหรับ TLS 1.2 - ชุมชนด้านเทคนิคของ Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server ส่วนแนวทาง TLS ที่ 2: การเปิดใช้งาน TLS 1.2 และไคลเอ็นต์ที่ระบุที่ไม่ได้ใช้ - ชุมชนด้านเทคนิคของ Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [การความเข้าใจสถานการณ์อีเมลถ้าเวอร์ชัน TLS ไม่สามารถยอมรับExchange Online - ชุมชนด้านเทคนิคของ Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
