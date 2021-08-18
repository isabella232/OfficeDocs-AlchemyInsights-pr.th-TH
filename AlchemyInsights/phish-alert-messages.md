---
title: 2491 ข้อความแจ้งเตือนข้อความอีเมลจากนโยบาย 'ส่งโดย Phish เนื่องจากผู้เช่าหรือการแทนที่ผู้ใช้'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316377"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>การแจ้งเตือนข้อความอีเมลจากนโยบาย 'ส่งโดย Phish เนื่องจากผู้เช่าหรือการแทนที่ผู้ใช้'

นโยบายการแจ้งเตือนเริ่มต้นที่ชื่อ **Phish Delivered เนื่องจากผู้เช่าหรือการแทนที่** ผู้ใช้พร้อมใช้งานในองค์กรที่มีสิทธิ์การใช้งาน Microsoft Defender Office 365 P1 และ P2 ถ้าคุณได้รับการแจ้งเตือนนี้ ต่อไปนี้คือขั้นตอนในการตรวจสอบ

1. จากข้อความแจ้งเตือน ให้คลิก **ดูการแจ้งเตือน** เพื่อ **ไปที่หน้า** การแจ้งเตือน Microsoft 365 Defenderการแจ้งเตือน

2. เลือกการแจ้งเตือนเพื่อดูตัวเลือกในการ **ดูรายการข้อความ หรือ****ดูข้อความใน Explorer** ตัวเลือกทั้งสองตัวเลือกจะพาคุณไปยังรายละเอียดของข้อความ ซึ่งรวมถึง ID ข้อความ โปรดทราบว่าลิงก์ Threat Explorer จะกรองข้อความที่ตรงกับเกณฑ์การแจ้งเตือนโดยอัตโนมัติ คุณอาจต้องปรับตัวกรองวันที่ใน Threat Explorer

ข้อความฟิชชิ่งถูกส่งเนื่องจากการแทนที่ที่กําหนดค่าด้วยตนเอง:

- ผู้ส่งหรือโดเมนที่อนุญาตที่ตั้งค่าโดยผู้ใช้
- ผู้ส่งหรือโดเมนที่อนุญาตที่ตั้งค่าโดยผู้ดูแลระบบในนโยบายการป้องกันสแปม
- ที่อยู่ IP ที่อนุญาตในนโยบายตัวกรองการเชื่อมต่อ
- กฎล.ก.ล.ต. จดหมาย (หรือที่เรียกว่ากฎการส่งผ่าน) ที่ถูกกําหนดค่าให้อนุญาตข้อความ

ถ้าคุณเชื่อว่าข้อความถูกระบุว่าเป็นฟิชชิ่งอย่างไม่ถูกต้อง ให้ใช้การส่ง [ของผู้ดูแลระบบ](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) เพื่อรายงานข้อความไปยังไมโครซอฟท์

ผู้ใช้สามารถใช้[Add-in ของข้อความรายงานหรือ Add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)ฟิชชิ่งของรายงาน Outlookเพื่อส่งตัวอย่างข้อความไปยังไมโครซอฟท์ได้
