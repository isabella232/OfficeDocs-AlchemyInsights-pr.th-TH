---
title: การแก้ไขปัญหาข้อผิดพลาดผลิตภัณฑ์ที่ไม่มีใบอนุญาต
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786868"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>ข้อเสนอแนะเพื่อแก้ไขข้อผิดพลาด "ผลิตภัณฑ์ที่ไม่มีใบอนุญาต"

เมื่อต้องการแก้ไขข้อผิดพลาดเกี่ยวกับ "ผลิตภัณฑ์ที่ไม่มีใบอนุญาต" ให้ลองใช้วิธีต่อไปนี้:

- ตรวจสอบเพื่อดูว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่
- ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตสิทธิ์การใช้งานไคลเอ็นต์ เช่น แอป Microsoft 365 For Business หรือ Business Premium และตรวจสอบให้แน่ใจว่า [ผู้ใช้ได้รับการมอบหมาย](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)สิทธิ์การใช้งาน 
- ตรวจสอบให้แน่ใจว่าผู้ใช้ลงชื่อเข้าใช้ Office ด้วยบัญชีเดียวกันกับที่ได้รับการมอบหมายสิทธิ์การใช้งาน
- ตรวจสอบ [หน้า สถานภาพ](https://docs.microsoft.com/office365/enterprise/view-service-health) บริการ เพื่อดูว่ามีปัญหาที่ทราบเกี่ยวกับบริการหรือไม่
- ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าไม่ได้บล็อกไม่ให้แอป Microsoft 365 เข้าถึงอินเทอร์เน็ต ดู [URL และช่วงที่อยู่](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)IP

คุณอาจลองแก้ไขปัญหาต่อไปนี้: 

- เปิดแอป Office [แล้วลงชื่อ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) ออกจากบัญชีผู้ใช้ใดๆ ที่มีอยู่ [เอาออก](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)[และกําหนด](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)สิทธิ์การใช้งาน Office ใหม่[แล้วลงชื่อเข้าใช้ Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ
- เรียกใช้ [ตัวแก้ไขปัญหา](https://aka.ms/SARA-OfficeActivation-Alchemy)การเปิดใช้งาน
- [รีเซ็ตสถานะการเปิดใช้งาน Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state) 
- [ซ่อมแซมแบบออนไลน์ของ Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)

ดูวิธีแก้ไขปัญหาเพิ่มเติมที่: 

- [ข้อผิดพลาดผลิตภัณฑ์ที่ไม่มีใบอนุญาตและการเปิดใช้งานใน Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- ["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง" ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)