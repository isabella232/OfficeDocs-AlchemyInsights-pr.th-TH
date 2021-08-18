---
title: แก้ไขปัญหาทั่วไปเกี่ยวกับการจัดรูปแบบระเบียน DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324009"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>แก้ไขปัญหาทั่วไปเกี่ยวกับการจัดรูปแบบระเบียน DKIM

ปัญหาการตั้งค่า DKIM ส่วนใหญ่เกี่ยวข้องกับระเบียน DNS ที่ไม่ถูกต้อง

เมื่อต้องการแก้ไขปัญหาการตั้งค่า DKIM ให้ตรวจสอบว่าระเบียน CNAME ของ DKIM (**ไม่ใช่** ระเบียน TXT) ได้รับการจัดรูปแบบอย่างถูกต้อง หากต้องการข้อมูลเพิ่มเติม โปรดดู[สิ่งที่คุณต้องใช้ในการตั้งค่า DKIM ด้วยตนเองใน Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

ถ้าคุณต้องการความช่วยเหลือเกี่ยวกับระเบียน DNS โดยทั่วไป ให้ดูที่ สร้างระเบียน[DNS ที่ผู้ให้บริการโฮสต์ DNS ใดๆ Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

**หมายเหตุ**: หลังจากที่คุณสร้างหรืออัปเดตระเบียน DNS DKIM ของคุณที่บริการการโฮสต์ DNS ของโดเมนของคุณแล้ว คุณจะต้องรอให้ระเบียน DNS เผยแพร่
