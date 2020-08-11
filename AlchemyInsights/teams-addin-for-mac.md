---
title: Add-in ของทีมสำหรับ Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629967"
---
# <a name="teams-add-in-for-mac"></a>Add-in ของทีมสำหรับ Mac

เมื่อต้องการแก้ไขปัญหาสำหรับผู้ใช้ระบบปฏิบัติการของระบบปฏิบัติการของ Mac ที่ขาดหายไปให้ทำตามขั้นตอนต่อไปนี้:

**ขั้นตอนที่ 1:** ถ้าคุณมี Exchange แบบไฮบริดในองค์กร (๒๐๑๖ CU3 หรือใหม่กว่าที่จำเป็น) ให้ใช้เครื่องมือ Test-HMA.ps1 เพื่อยืนยันว่าการรับรองความถูกต้องแบบไฮบริดที่ทันสมัยถูกกำหนดค่าอย่างถูกต้อง สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[ตรวจสอบการตั้งค่าการรับรองความถูกต้องแบบไฮบริดที่ทันสมัยสำหรับ Outlook สำหรับ iOS และ Android](https://aka.ms/AA980zq)  

**หมายเหตุ:** ใช้รูปแบบที่อยู่ UPN (ตัวอย่างเช่น[username@contoso.com](mailto:username@contoso.com)), not domain\username. ให้ทำสิ่งนี้แม้แต่สำหรับผู้ใช้ที่มีกล่องจดหมาย Exchange Online

**ขั้นตอนที่ 2:** มีผู้ใช้ไปที่**บัญชีเครื่องมือ**  >  **Accounts**... ใน Outlook for Mac และค้นหาและเลือกบัญชีผู้ใช้ ยืนยันชื่อผู้ใช้ที่แสดงอยู่ในรูปแบบ UPN (ตัวอย่างเช่น[username@contoso.com](mailto:username@contoso.com))

**ขั้นตอนที่ 3:** ยืนยันผู้ใช้เป็นผู้ใช้ Microsoft team ที่ได้รับสิทธิ์การใช้งาน ผู้ใช้ต้องใช้การสมัครใช้งาน Office ๓๖๕ for Mac เวอร์ชันผลิตภัณฑ์๑๖.๒๔หรือเวอร์ชันที่ใหม่กว่า