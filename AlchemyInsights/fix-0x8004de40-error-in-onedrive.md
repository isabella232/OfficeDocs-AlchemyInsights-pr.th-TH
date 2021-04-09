---
title: แก้ไขข้อผิดพลาด 0x8004de40 ใน OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649767"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>แก้ไขข้อผิดพลาด 0x8004de40 ใน OneDrive

ถ้าคุณเรียกใช้ Windows 7 และได้รับข้อผิดพลาดนี้ อัปเดตเพื่อเปิดใช้งาน[TLS 1.1 และ TLS 1.2 เป็นโพรโทคอลที่ปลอดภัยเริ่มต้นใน WinHTTP ใน Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

ถ้าคุณใช้งาน Windows 10 และคุณได้รับข้อผิดพลาด0x8004de40 OneDrive:

- เริ่มระบบคอมพิวเตอร์ที่ได้รับผลกระทบใหม่ขณะเชื่อมต่อกับโดเมนไดเรกทอรี Acitve ของคุณ
- ถ้าการเริ่มต้นระบบใหม่ไม่สามารถแก้ไขปัญหาได้ ให้ยกเลิกการเข้าร่วมและเข้าร่วมอุปกรณ์ของคุณอีกครั้งจาก Azure AD 

**หมายเหตุ**: คุณควรอยู่บนเครือข่ายขององค์กรขณะปฏิบัติตามขั้นตอนเหล่านี้ อย่าปฏิบัติตามขั้นตอนเหล่านี้เมื่อคุณไม่ได้เชื่อมต่อกับโครงสร้างพื้นฐานของบริษัทของคุณ (ตัวอย่างเช่น ขณะเดินทาง) 

1. เปิดพร้อมท์ของสั่งด้วยสิทธิ์ผู้ดูแล **โดย** การเลือก เริ่ม คลิกขวาที่ **พร้อมท์** สั่ง **แล้วเลือก เรียกใช้ในฐานะ** ผู้ดูแลระบบ

1. พิมพ์ *dsregcmd /leave* แล้วกด **Enter**

1. เมื่อเสร็จสมบูรณ์ ให้พิมพ์ *dsregcmd /join* แล้วกด **Enter**

1. เมื่อเสร็จสมบูรณ์ ให้ปิดพร้อมท์ของสั่ง

1. เริ่มระบบคอมพิวเตอร์ใหม่ แล้วเข้าสู่ระบบ OneDrive