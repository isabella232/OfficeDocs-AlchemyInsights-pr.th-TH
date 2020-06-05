---
title: การแก้ไขข้อผิดพลาดผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งาน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: 89d0e589329d40f17c36baa54868154be0f5b887
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582758"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>คําแนะนําสําหรับการแก้ปัญหาข้อผิดพลาด "ผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งาน"

เมื่อต้องการแก้ไขข้อผิดพลาดเกี่ยวกับ "ผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งาน" ให้ลองทําดังต่อไปนี้

- ตรวจสอบว่าสถานะการสมัครใช้งานของคุณหมดอายุแล้วหรือไม่
- ตรวจสอบให้แน่ใจว่าคุณมีการสมัครใช้งานที่อนุญาตให้มีสิทธิ์การใช้งานไคลเอ็นต์ เช่น Microsoft 365 Apps สําหรับธุรกิจหรือ Business Premium และ[ตรวจสอบว่าผู้ใช้มีสิทธิ์การใช้งานที่ได้รับมอบหมาย](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) 
- ตรวจสอบให้แน่ใจว่า ผู้ใช้ลงชื่อเข้าใช้ Office ด้วยบัญชีผู้ใช้เดียวกันกับที่มีการกําหนดสิทธิ์การใช้งาน
- ตรวจสอบ[หน้าสถานภาพบริการ](https://docs.microsoft.com/office365/enterprise/view-service-health)เพื่อดูว่ามีปัญหาใด ๆ ที่ทราบเกี่ยวกับบริการหรือไม่
- ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าไฟร์วอลล์ของคุณไม่ได้บล็อกการเข้าถึงแอป Microsoft 365 ไปยังอินเทอร์เน็ต ดู[URL และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

นอกจากนี้คุณอาจลองการดําเนินการแก้ไขปัญหาต่อไปนี้: 

- เปิดแอป Office และ[ออกจากระบบ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)บัญชีผู้ใช้ที่มีอยู่ [เอาออก](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users)และมอบหมายสิทธิ์การใช้งาน Office[แล้ว](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)[เข้าสู่ระบบ Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)โดยใช้บัญชีผู้ใช้ได้รับผลกระทบ
- เรียกใช้[ตัวแก้ไขปัญหาการเปิดใช้งาน](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [รีเซ็ตสถานะการเปิดใช้งาน Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state) 
- [ดําเนินการซ่อมแซม Office แบบออนไลน์](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)

สําหรับการแก้ไขปัญหาเพิ่มเติม โปรดดู: 

- [ผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งานและข้อผิดพลาดในการเปิดใช้งานใน Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- ["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณ โปรดลองอีกครั้งในภายหลัง"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)