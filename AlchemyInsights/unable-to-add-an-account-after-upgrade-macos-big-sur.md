---
title: ไม่สามารถเพิ่มบัญชีหลังการอัปเกรดเป็น macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506759"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>ไม่สามารถเพิ่มบัญชีหลังการอัปเกรดเป็น macOS 11.6 Big Sur

หลังจากอัปเกรดเป็น macOS 11.6 แล้ว บัญชี OneDrive ของคุณที่โรงเรียนหรือบัญชี OneDrive ส่วนบุคคลของคุณอาจไม่ปรากฏในรายการบัญชีของคุณ และคุณอาจไม่สามารถเข้าสู่ระบบบัญชีที่สองจากแอปได้

การแก้ไขปัญหานี้ได้รับการพัฒนาขึ้น ก่อนอื่น ให้ระบุว่า คุณใช้งานเวอร์ชันสแตนด์อโลนหรือ App Store ของ OneDrive:

- เลือกOneDrive Cloud ในแถบเมนู>**วิธีใช้& การตั้งค่า**  >  **การตั้งค่า**  >  เกี่ยวกับ หากหมายเลขเวอร์ชันไม่มี **(แบบสแตนด์อโลน)** คุณมีผลิตภัณฑ์เวอร์ชัน App Store

ถ้าคุณใช้งานเวอร์ชันสแตนด์OneDriveโลน ให้รีสตาร์ตเครื่องของคุณ OneDriveอัปเดตอัตโนมัติเป็นรุ่นที่ปัญหานี้ได้รับการแก้ไข ถ้าคุณต้องการติดตั้งรุ่นด้วยตนเอง ให้ดาวน์โหลดไฟล์[.zip ไฟล์](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)unzip ไฟล์ และคัดลอกแอป OneDrive ลงในโฟลเดอร์ แอปพลิเคชัน (โดยการแทนที่แอป OneDrive ที่มีอยู่)

ถ้าคุณใช้งานเวอร์ชัน App Store ให้พิจารณาติดตั้งเวอร์ชันสแตนด์อโลนOneDriveเวอร์ชัน เวอร์ชันนี้ใช้งานได้แบบเดียวกับเวอร์ชัน App Store แต่ช่วยให้ไมโครซอฟท์สามารถเสนอการอัปเดตได้รวดเร็วยิ่งขึ้นกับผู้ใช้และเชื่อมต่อกับเวอร์ชันที่มีการแก้ไขปัญหานี้

1. ดาวน์โหลดเวอร์ชันสแตนด์OneDrive[โลนที่มี](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)การแก้ไข
2. Unzip ไฟล์ และคัดลอกOneDriveลงในโฟลเดอร์แอปพลิเคชัน (โดยการแทนที่แอปOneDriveที่มีอยู่)

ถ้าคุณต้องการใช้เวอร์ชัน App Store ให้รอให้ App Store เผยแพร่เวอร์ชันของแอปที่รวมการแก้ไข น่าเสียดายที่ Microsoft ไม่สามารถแจ้งวันที่โดยประมาณให้เผยแพร่เวอร์ชันที่แก้ไขแล้วจาก App Store ได้


