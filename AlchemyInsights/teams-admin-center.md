---
title: ศูนย์การจัดการ Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826398"
---
# <a name="teams-admin-center"></a>ศูนย์การจัดการ Teams

เรียนรู้เกี่ยวกับการจัดการ Teams ด้วย [ศูนย์การจัดการ](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center)Teams

ถ้าคุณไม่สามารถเข้าถึงศูนย์การจัดการ Teams โปรดตรวจสอบรายการต่อไปนี้:

- ตรวจสอบว่าคุณได้อนุญาตที่อยู่ [IP และ URL ของ Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) ที่เหมาะสมบนอุปกรณ์เฉพาะเขตใดๆ (ไฟร์วอลล์ และอื่นๆ) หรือในกฎไฟร์วอลล์บนเครื่องคอมพิวเตอร์ของคุณ
- ตรวจสอบว่าการเข้าสู่ระบบที่คุณใช้เพื่อเข้าถึงพอร์ทัลการดูแลระบบ Teams ตรงกับชื่อผู้ใช้ของคุณที่แสดงในพอร์ทัล[ผู้ดูแลระบบ Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)

ถ้าผู้ใช้ไม่ปรากฏในศูนย์การจัดการ Teams โปรดตรวจสอบสิ่งต่อไปนี้:

- คุณได้สร้างผู้ใช้หรือสิทธิ์การใช้งานที่ได้รับมอบหมายใน 24 ชั่วโมงที่ผ่านมาแล้วหรือยัง โปรดตรวจสอบให้แน่ใจว่าคุณรออย่างน้อย 24 ชั่วโมงก่อนที่จะเปิดตั๋วการสนับสนุน
- ตรวจสอบว่าคุณได้มอบหมายสิทธิ์การใช้งานที่เหมาะสมหรือไม่
- ถ้าคุณมี Active Directory ภายในองค์กร ให้ตรวจสอบว่าค่าของ [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress)หรือที่อยู่ SIP ในเขตข้อมูล ProxyAddresses ใน Active Directory ภายในเครื่องของคุณไม่ซ้ิอกัน และรูปแบบตรงกับ **sip:** ชื่อผู้ใช้ของผู้ใช้จากศูนย์การจัดการ [Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- ถ้าคุณต้องการเก็บการปรับใช้ Skype for Business Server และให้ผู้ใช้อยู่ในองค์กรและออนไลน์: ติดตาม "ตั้งค่าแบบไฮบริดกับ Teams และ **Skype for Business Online"** ในแผงควบคุม Skype for Business Server ของคุณ และย้ายผู้ใช้ออนไลน์
