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
ms.openlocfilehash: 7922a2c5306f9d16856502b5e57e585cb90f2f7c9abaad0366f72ed46de786d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957119"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>ข้อเสนอแนะเพื่อแก้ไขข้อผิดพลาด "ผลิตภัณฑ์ที่ไม่มีใบอนุญาต"

เมื่อต้องการแก้ไขข้อผิดพลาดเกี่ยวกับ "ผลิตภัณฑ์ที่ไม่มีใบอนุญาต" ให้ลองใช้วิธีต่อไปนี้:

- ตรวจสอบเพื่อดูว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่
- ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตสิทธิ์การใช้งานไคลเอ็นต์ เช่น Microsoft 365 Apps for business หรือ Business Premium และตรวจสอบให้แน่ใจว่า[ผู้ใช้ได้รับ](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)สิทธิ์การใช้งาน 
- ตรวจสอบให้แน่ใจว่าผู้ใช้ลงชื่อเข้าใช้Officeด้วยบัญชีเดียวกันกับที่ได้รับการมอบหมายสิทธิ์การใช้งาน
- ตรวจสอบ [หน้า สถานภาพ](https://docs.microsoft.com/office365/enterprise/view-service-health) บริการ เพื่อดูว่ามีปัญหาที่ทราบเกี่ยวกับบริการหรือไม่
- ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าไม่ได้บล็อกMicrosoft 365การเข้าถึงอินเทอร์เน็ต ดู [URL และช่วงที่อยู่](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)IP

คุณอาจลองแก้ไขปัญหาต่อไปนี้: 

- เปิดแอป Office[และ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)ลงชื่อออกจากบัญชีผู้ใช้ใดๆ ที่มีอยู่ [เอาออก](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)[และกําหนดOffice](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)สิทธิ์การใช้งานใหม่[แล้วOffice](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ
- เรียกใช้ [ตัวแก้ไขปัญหา](https://aka.ms/SARA-OfficeActivation-Alchemy)การเปิดใช้งาน
- [รีเซ็ตOfficeสถานะการเปิดใช้งาน](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state) 
- [ซ่อมแซมแบบออนไลน์ ของ Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)

ดูวิธีแก้ไขปัญหาเพิ่มเติมที่: 

- [ข้อผิดพลาดผลิตภัณฑ์ที่ไม่มีใบอนุญาตและการเปิดใช้งานในOffice](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- ["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง" ข้อผิดพลาดเมื่อคุณOffice](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)