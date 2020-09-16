---
title: ไม่สามารถเปิดใช้งาน Office ได้
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
- "2000023"
- "3509"
ms.openlocfilehash: 50939456df57920994e464db20e5da54f45f197a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744645"
---
# <a name="unable-to-activate-office"></a>ไม่สามารถเปิดใช้งาน Office ได้

- ตรวจสอบว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่
- ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตให้ใช้สิทธิ์การใช้งานไคลเอ็นต์เช่น Office ๓๖๕ Business หรือ Business Premium และ [ตรวจสอบให้แน่ใจว่าผู้ใช้มีสิทธิ์](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users)การใช้งานที่ได้รับมอบหมาย
- ตรวจสอบให้แน่ใจว่าผู้ใช้กำลังลงชื่อเข้าใช้ Office ด้วยบัญชีผู้ใช้เดียวกันกับสิทธิ์การใช้งานที่ได้รับมอบหมาย
- ตรวจสอบ [หน้าสถานภาพบริการของ Office ๓๖๕](https://docs.microsoft.com/office365/enterprise/view-service-health) เพื่อดูว่ามีปัญหาที่ทราบเกี่ยวกับบริการหรือไม่
- ตรวจสอบไฟร์วอลล์ซอฟต์แวร์ป้องกันไวรัสและการตั้งค่าพร็อกซีของคุณเพื่อยืนยันว่าพวกเขาไม่ได้บล็อก Microsoft ๓๖๕ apps access ไปยังอินเทอร์เน็ต โปรดดู[ที่ url และช่วงที่อยู่ IP ของ Office ๓๖๕](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Url และช่วงที่อยู่ IP ของ Office ๓๖๕")

ใช้การดำเนินการแก้ไขปัญหาต่อไปนี้:

- เปิดแอป Office และ [ลงชื่อออก](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) จากบัญชีผู้ใช้ใดๆที่มีอยู่ [เอาออก](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) และกำหนดสิทธิ์การใช้งาน Office [อีกครั้ง](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) แล้ว [ลงชื่อ](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) เข้าใช้ office โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ
- เรียกใช้ตัว [แก้ไขปัญหาการเปิดใช้งาน](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่")
- [ดำเนินการซ่อมแซมแบบออนไลน์ของ Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

สำหรับโซลูชันการแก้ไขปัญหาเพิ่มเติมให้ดูที่:  

- [ข้อผิดพลาดในการเปิดใช้งานผลิตภัณฑ์และการเปิดใช้งานใน Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- ["ขออภัยเราไม่สามารถเชื่อมต่อกับบัญชีผู้ใช้ของคุณได้ โปรดลองอีกครั้งในภายหลัง "ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)