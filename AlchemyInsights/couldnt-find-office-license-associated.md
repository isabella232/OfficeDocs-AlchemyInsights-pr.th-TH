---
title: การแก้ไขแอป Microsoft ๓๖๕ไม่สามารถค้นหาข้อความที่เกี่ยวข้องกับสิทธิ์การใช้งาน office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747714"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>การแก้ไขข้อความ Microsoft ๓๖๕ apps "ไม่พบสิทธิ์การใช้งาน office ที่เกี่ยวข้อง"

ถ้าคุณได้รับข้อความนี้ให้ลองทำดังต่อไปนี้:

1. ตรวจสอบไฟร์วอลล์ซอฟต์แวร์ป้องกันไวรัสและการตั้งค่าพร็อกซีของคุณเพื่อยืนยันว่าพวกเขาไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Microsoft ๓๖๕ ให้ดู[ที่ url และช่วงที่อยู่ IP ของ Microsoft ๓๖๕](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. เอาออกและ [กำหนดสิทธิ์การใช้งาน Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ใหม่สำหรับผู้ใช้ที่ได้รับผลกระทบ 
3. เปิดแอป Office และ [ลงชื่อออกจาก](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) บัญชีผู้ใช้ใดๆที่มีอยู่
4. ไปที่การตั้งค่า Windows >**บัญชี**ผู้  >  ใช้**อีเมลของ**บัญชีผู้ใช้ & และเอาบัญชีผู้ใช้ที่ทำงานทั้งหมดออกยกเว้นบัญชีที่ได้รับผลกระทบ
5. ไปที่การตั้งค่า**Accounts**Windows > การ  >  **เข้าถึงบัญชีผู้ใช้ที่ทำงานหรือโรงเรียน**และยกเลิกการเชื่อมต่อบัญชีที่ทำงานทั้งหมดยกเว้นบัญชีที่ได้รับผลกระทบ
6. ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่ [เรียนรู้วิธี](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)การ
7. [ลงชื่อเข้า](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) ใช้โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ

สำหรับโซลูชันการแก้ไขปัญหาเพิ่มเติมให้ดู[ที่ข้อผิดพลาดในการเปิดใช้งานผลิตภัณฑ์และการเปิดใช้งานใน Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)