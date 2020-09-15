---
title: ศูนย์การจัดการทีม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670383"
---
# <a name="teams-admin-center"></a>ศูนย์การจัดการทีม

เรียนรู้เกี่ยวกับการจัดการทีมด้วย[ศูนย์การจัดการทีม](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center)

ถ้าคุณไม่สามารถเข้าถึงศูนย์การจัดการทีมโปรดตรวจสอบรายการต่อไปนี้:

- ตรวจสอบว่าคุณได้อนุญาตให้ใช้ที่ [อยู่ IP ของ Office ๓๖๕](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) ที่เหมาะสมและ URL บนอุปกรณ์ขอบเขตใดก็ได้ (ไฟร์วอลล์ฯลฯ) หรือในกฎไฟร์วอลล์บนเครื่องคอมพิวเตอร์ของคุณ
- ตรวจสอบว่าการเข้าสู่ระบบที่คุณใช้ในการเข้าถึงพอร์ทัลผู้ดูแลระบบของทีมตรงกับชื่อผู้ใช้ของคุณที่แสดงรายการอยู่ใน[พอร์ทัลผู้ดูแลระบบ Microsoft ๓๖๕](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)

ถ้าผู้ใช้ไม่ปรากฏในศูนย์การจัดการทีมโปรดตรวจสอบสิ่งต่อไปนี้:

- คุณสร้างผู้ใช้หรือสิทธิ์การใช้งานที่มอบหมายใน24ชั่วโมงที่ผ่านมาหรือไม่ โปรดตรวจสอบให้แน่ใจว่าคุณรออย่างน้อย24ชั่วโมงก่อนที่จะเปิดบัตรสนับสนุน
- ตรวจสอบว่าคุณได้กำหนดสิทธิ์การใช้งานที่เหมาะสมแล้วหรือยัง
- ถ้าคุณมีไดเรกทอรีที่ใช้งานอยู่ภายในองค์กรให้ตรวจสอบว่า[ค่าของ msRTCSIP-PrimaryUserAddress หรือที่อยู่ SIP ในเขตข้อมูล ProxyAddresses ใน Active directory ภายในเครื่องของคุณจะไม่ซ้ำกันและรูปแบบที่ตรงกับ](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress)SIP:**ชื่อ**ผู้ใช้ของผู้ใช้จาก[ศูนย์การจัดการ Microsoft ๓๖๕](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- ถ้าคุณต้องการเก็บการปรับใช้ Skype for Business Server และมีผู้ใช้ที่ homed ภายในองค์กรและออนไลน์: ให้ทำตามขั้นตอน **"ตั้งค่าไฮบริดที่มีทีมและ skype For Business Online"** ในแผงควบคุมเซิร์ฟเวอร์ Skype for business ของคุณและย้ายผู้ใช้แบบออนไลน์
