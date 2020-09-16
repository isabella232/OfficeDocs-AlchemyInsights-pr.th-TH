---
title: อีเมลขาออกไปยังโฟลเดอร์อีเมลขยะ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769202"
---
# <a name="outbound-email-to-junk-email-folder"></a>อีเมลขาออกไปยังโฟลเดอร์อีเมลขยะ

ถ้าคุณเห็นข้อความขาออกที่ถูกทำเครื่องหมายเป็นอีเมลขยะให้ทำตามขั้นตอนต่อไปนี้:

- ถ้าคุณยังไม่ได้ทำให้ลอง[กำหนดค่าการแจ้งให้ทราบเกี่ยวกับนโยบายสแปมขาออก](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)

- ใช้การ[ติดตามข้อความ](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc)เพื่อดูว่าข้อความขาออกมีค่าอี**เมลสแปม**ที่มีรายละเอียดเพิ่มเติมหรือไม่ให้**ใช้กลุ่มการจัดส่งที่มีความเสี่ยงสูง**

  สำหรับข้อความเหล่านี้ให้ตรวจสอบเนื้อหาข้อความเพื่อดูสิ่งที่อาจถือว่าเป็นสแปม ตัวอย่างเช่นลายเซ็นบางครั้งอาจทำให้เกิดปัญหาสำหรับผู้ใช้หลายคน

  ถ้าคุณมีหลายตัวอย่างของข้อความขาออกที่ถูกทำเครื่องหมายว่าเป็นอีเมลขยะให้เปิดบัตรสนับสนุนและขอให้เจ้าหน้าที่สนับสนุนส่งข้อความของคุณเป็น false บวกไปถึงนักวิเคราะห์สแปมของเรา เตรียมพร้อมที่จะให้ข้อความตัวอย่างที่มีส่วนหัวของข้อความทั้งหมด
