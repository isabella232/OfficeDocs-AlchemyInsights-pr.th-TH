---
title: ไม่สามารถเปิดใช้งาน Office ได้
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
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812591"
---
# <a name="unable-to-activate-office"></a>ไม่สามารถเปิดใช้งาน Office ได้

- ตรวจสอบว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่
- ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตสิทธิ์การใช้งานไคลเอ็นต์ เช่น Office 365 Business หรือ Business Premium และตรวจสอบ[ให้แน่ใจว่าผู้ใช้ได้รับการมอบหมายสิทธิ์การใช้งาน](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide)
- ตรวจสอบให้แน่ใจว่าผู้ใช้ลงชื่อเข้าใช้ Office ด้วยบัญชีเดียวกันกับที่ได้รับการมอบหมายสิทธิ์การใช้งาน
- ตรวจสอบ [หน้า สถานภาพบริการของ Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) เพื่อดูว่ามีปัญหาที่ทราบเกี่ยวกับบริการหรือไม่
- ตรวจสอบการตั้งค่าไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และพร็อกซีเพื่อยืนยันว่าไม่ได้บล็อกไม่ให้แอป Microsoft 365 เข้าถึงอินเทอร์เน็ต โปรดดู[URL และช่วงที่อยู่ IP ของ Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL และช่วงที่อยู่ IP ของ Office 365")

**เคล็ดลับ** บนเครื่อง Windows เราสามารถวินิจฉัยและแก้ไขปัญหาการลงชื่อเข้าใช้ Office ทั่วไปหลายอย่างให้คุณโดยอัตโนมัติ ดาวน์โหลดและเรียกใช้  **[ตัวช่วยการสนับสนุนและการกู้คืน](https://aka.ms/SaRA-OfficeSignInScenario)** ของ Microsoft เพื่อใช้เครื่องมืออัตโนมัติของเรา

ใช้การแอคชันการแก้ไขปัญหาต่อไปนี้

- เปิดแอป Office [แล้วลงชื่อ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) ออกจากบัญชีผู้ใช้ใดๆ ที่มีอยู่ [ลบ](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)[แล้วมอบหมายสิทธิ์การใช้งาน](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)Office ใหม่[แล้วลงชื่อเข้าใช้ Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ
- เรียกใช้ [ตัวแก้ไขปัญหาการเปิดใช้งาน](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่")
- [ซ่อมแซมแบบออนไลน์ของ Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

ดูวิธีแก้ไขปัญหาเพิ่มเติมที่:  

- [ข้อผิดพลาดผลิตภัณฑ์ที่ไม่มีใบอนุญาตและการเปิดใช้งานใน Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- ["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง" ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)