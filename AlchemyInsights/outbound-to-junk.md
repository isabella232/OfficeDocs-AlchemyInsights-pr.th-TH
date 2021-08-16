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
ms.openlocfilehash: 52aa5aa86848fa92ac082e8f672f9f501cd97cf2f3db9c40fa745aa8ebccfbb1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54096677"
---
# <a name="outbound-email-to-junk-email-folder"></a>อีเมลขาออกไปยังโฟลเดอร์อีเมลขยะ

ถ้าคุณเห็นข้อความขาออกที่ถูกระบุว่าเป็นอีเมลขยะ ให้ปฏิบัติตามขั้นตอนต่อไปนี้

- ถ้าคุณยังไม่ได้กําหนดค่า ให้พิจารณา [การกําหนดค่าการแจ้งเตือนนโยบายสแปม](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)ขาออก

- ใช้ [การติดตาม](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) ข้อความเพื่อดูว่าข้อความขาออกมีค่าเหตุการณ์ **สแปมและมีรายละเอียด** เพิ่มเติมหรือไม่: **ใช้พูลการส่งอีเมลมีความเสี่ยง** สูง

  ข้อความเหล่านี้ ให้ตรวจสอบเนื้อหาข้อความเพื่อดูว่าข้อความใดที่อาจได้รับการพิจารณาว่าเป็นสแปม ตัวอย่างเช่น บางครั้งลายเซ็นอาจทําให้เกิดปัญหากับผู้ใช้หลายคน

  ถ้าคุณมีหลายตัวอย่างของข้อความขาออกที่ถูกต้องที่ถูกระบุว่าเป็นอีเมลขยะ ให้เปิดตั๋วการสนับสนุนและขอให้ตัวแทนฝ่ายสนับสนุนส่งข้อความของคุณเป็นค่าบวกที่ผิดไปยังนักวิเคราะห์สแปมของเรา เตรียมพร้อมเพื่อให้ข้อความตัวอย่างที่มีส่วนหัวของข้อความทั้งหมด
