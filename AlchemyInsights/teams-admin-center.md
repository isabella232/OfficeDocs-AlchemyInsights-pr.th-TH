---
title: Teams ศูนย์การจัดการ
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
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049363"
---
# <a name="teams-admin-center"></a>Teams ศูนย์การจัดการ

เรียนรู้เกี่ยวกับTeamsด้วย[Teamsผู้ดูแลระบบ](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center)

ถ้าคุณไม่สามารถเข้าถึงศูนย์การจัดการ Teamsได้ โปรดตรวจสอบรายการต่อไปนี้:

- ตรวจสอบว่าคุณได้อนุญาตให้มีที่อยู่ IP [Office 365และ URL ที่เหมาะสม](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service)บนอุปกรณ์เฉพาะเขตใดๆ (ไฟร์วอลล์ และอื่นๆ) หรือในกฎไฟร์วอลล์บนเครื่องคอมพิวเตอร์ของคุณ
- ตรวจสอบว่าการเข้าสู่ระบบที่คุณใช้เพื่อเข้าถึงพอร์ทัลการดูแลระบบTeamsที่ตรงกับชื่อผู้ใช้ของคุณซึ่งแสดงรายการ[การจัดการ Microsoft 365พอร์ทัล](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)

ถ้าผู้ใช้ไม่ปรากฏอยู่ในศูนย์Teamsศูนย์การจัดการ โปรดตรวจสอบสิ่งต่อไปนี้:

- คุณได้สร้างผู้ใช้หรือสิทธิ์การใช้งานที่ได้รับมอบหมายใน 24 ชั่วโมงที่ผ่านมาแล้วหรือยัง โปรดตรวจสอบให้แน่ใจว่าคุณรออย่างน้อย 24 ชั่วโมงก่อนที่จะเปิดตั๋วการสนับสนุน
- ตรวจสอบว่าคุณได้มอบหมายสิทธิ์การใช้งานที่เหมาะสมหรือไม่
- ถ้าคุณมี Active Directory ภายในองค์กร ให้ตรวจสอบว่าค่าของ [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress)หรือที่อยู่ SIP ในเขตข้อมูล ProxyAddresses ใน Active Directory ภายในของคุณไม่ซ้ และรูปแบบตรงกับ **sip:** ชื่อผู้ใช้ของผู้ใช้จาก [ศูนย์การจัดการ Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- ถ้าคุณต้องการเก็บการปรับใช้งาน Skype for Business Server และให้ผู้ใช้อยู่ในองค์กรและออนไลน์: ให้ปฏิบัติตาม "ตั้งค่าแบบไฮบริดด้วย Teams และ **Skype for Business Online"** ในแผงควบคุม Skype for Business Server ของคุณ แล้วย้ายผู้ใช้แบบออนไลน์
