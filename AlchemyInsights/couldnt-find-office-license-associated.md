---
title: การแก้ไขแอป Office ไม่พบข้อความที่เกี่ยวข้องเกี่ยวกับสิทธิ์การใช้งาน Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 565df0a05baa974a6cbac58ac6be8d78470dbc5d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715651"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a>การแก้ไขข้อความ "ไม่พบสิทธิ์การใช้งาน Office ที่เกี่ยวข้อง"

ถ้าคุณได้รับข้อความนี้ ให้ลองทําดังต่อไปนี้:

1. ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าจะไม่บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Office ดู[URL ของ Microsoft 365 และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. เอาออก และ[กําหนดสิทธิ์การใช้งาน Office](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users)สําหรับผู้ใช้ที่ได้รับผลกระทบ 
3. เปิดแอป Office และ[ลงชื่อออกจาก](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)บัญชีผู้ใช้ที่มีอยู่
4. ไปที่ การตั้งค่า windows > > **บัญชีอีเมลบัญชี &** และเอาบัญชีการทํางานทั้งหมดยกเว้นบัญชีที่ได้รับผลกระทบ**Accounts**
5. ไปที่ การตั้งค่า Windows **>** > **ทํางานหรือโรงเรียนการเข้าถึง**และยกเลิกการเชื่อมต่อบัญชีที่ทํางานทั้งหมดยกเว้นบัญชีที่ได้รับผลกระทบ
6. ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่ [เรียนรู้วิธี](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [ลงชื่อเข้าใช้](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ

สําหรับการแก้ไขปัญหาเพิ่มเติม ให้ดูที่[ผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งานและข้อผิดพลาดในการเปิดใช้งานใน Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)