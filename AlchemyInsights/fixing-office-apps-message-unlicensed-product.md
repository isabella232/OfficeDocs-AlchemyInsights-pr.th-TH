---
title: ไม่สามารถเปิดใช้งานOffice
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
ms.openlocfilehash: eb62dfce9f9507dd8806d91343cd39fe76e65594473683c1393d524f6c2d8a27
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893930"
---
# <a name="unable-to-activate-office"></a>ไม่สามารถเปิดใช้งานOffice

**หมายเหตุ**: ถ้าคุณใช้งานเวอร์ชันที่เก่ากว่าWindows (ตัวอย่างเช่น Windows 7) ตรวจสอบให้แน่ใจว่าเปิดใช้งาน TLS 1.2 เป็นค่าเริ่มต้น For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

- ตรวจสอบว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่
- ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตสิทธิ์การใช้งานไคลเอ็นต์ เช่น Office 365 Business หรือ business Premium[และตรวจสอบให้แน่ใจว่าผู้ใช้ได้มอบหมายสิทธิ์การใช้งาน](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)
- ตรวจสอบให้แน่ใจว่าผู้ใช้ลงชื่อเข้าใช้Officeด้วยบัญชีเดียวกันกับที่ได้รับการมอบหมายสิทธิ์การใช้งาน
- ตรวจสอบ[Office 365สถานภาพ](https://docs.microsoft.com/office365/enterprise/view-service-health)บริการเพื่อดูว่ามีปัญหาที่ทราบเกี่ยวกับบริการหรือไม่
- ตรวจสอบการตั้งค่าไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และพร็อกซีของคุณเพื่อยืนยันว่าไม่ได้บล็อกMicrosoft 365ไม่ให้เข้าถึงอินเทอร์เน็ต โปรดดู[Office 365 URL และช่วงที่อยู่](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL และช่วงที่อยู่ IP")IP

**เคล็ดลับ** บนคอมพิวเตอร์Windows เราสามารถวินิจฉัยและแก้ไขปัญหาการลงชื่อเข้าใช้Officeทั่วไปต่างๆ ให้คุณโดยอัตโนมัติ ดาวน์โหลดและเรียกใช้ **[Microsoft ตัวช่วยการสนับสนุนและการกู้คืน](https://aka.ms/SaRA-OfficeSignInScenario)** เพื่อใช้เครื่องมืออัตโนมัติของเรา

ใช้การแก้ไขปัญหาต่อไปนี้

- เปิดแอป Office[และ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)ลงชื่อออกจากบัญชีผู้ใช้ใดๆ ที่มีอยู่ [เอาออก](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)[และ re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.
- เรียกใช้ [ตัวแก้ไขปัญหาการเปิดใช้งาน](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [ตั้งค่าสถานะOfficeเปิดใช้งานใหม่](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "ตั้งค่าสถานะOfficeเปิดใช้งานใหม่")
- [ใช้การซ่อมแซมแบบออนไลน์ของOffice](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

ดูวิธีแก้ไขปัญหาเพิ่มเติมที่:  

- [ข้อผิดพลาดผลิตภัณฑ์ที่ไม่มีใบอนุญาตและการเปิดใช้งานในOffice](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- ["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง" ข้อผิดพลาดเมื่อคุณOffice](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)