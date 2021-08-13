---
title: 305 เพิ่มขนาดกล่องจดหมายเก็บถาวร
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: f9cc968aba32645fd4433616618d096231ce4899e9e93335e802af5c05524a79
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926418"
---
# <a name="increase-the-archive-mailbox-size"></a>เพิ่มขนาดกล่องจดหมายเก็บถาวร


ถ้าคุณต้องการให้เราเรียกใช้การตรวจสอบการตั้งค่าที่กล่าวถึงด้านล่างโดยอัตโนมัติ ให้เลือกปุ่ม ย้อนกลับ < ที่ด้านบนของหน้านี้ แล้วใส่ที่อยู่อีเมลของผู้ใช้ที่ต้องการขนาดกล่องจดหมายเก็บถาวรของพวกเขาเพิ่มขึ้น

Microsoft 365จํากัดขนาดของกล่องจดหมาย[](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)เก็บถาวรโดยยึดตามสิทธิ์การใช้งานที่มอบหมายให้กับบัญชีผู้ใช้ เมื่อกล่องจดหมายเก็บถาวรถึง 90% ของขนาดที่อนุญาต ผู้ใช้จะได้รับการแจ้งเตือนทางอีเมล เมื่อกล่องจดหมายเก็บถาวรถึงขีดจํากัดขนาดแล้ว ผู้ใช้ไม่สามารถย้ายรายการเพิ่มเติมไปยังกล่องจดหมายเก็บถาวรได้ Microsoft 365จะไม่เพิ่มขนาดของกล่องจดหมายเก็บถาวรเมื่อถึงขีดจํากัดขนาดแล้ว แต่ผู้ใช้สามารถจัดการได้ดังต่อไปนี้เพื่อให้มีพื้นที่ว่างในกล่องจดหมายเก็บถาวร:

- ส่งออกรายการเป็นไฟล์ .pst โดยใช้Outlook

- ลบรายการออกจากกล่องจดหมายเก็บถาวร

Microsoft 365 **การเก็บถาวรแบบไม่Office 365 Enterprise** E3 และ E5 ผู้ดูแลระบบต้องเปิดใช้งานฟีเจอร์นี้ก่อนที่กล่องจดหมายเก็บถาวรจะมีขนาดสูงสุด เมื่อเปิดใช้งานการเก็บถาวรแบบไม่ต่ากัน อาจใช้เวลาถึง 30 วันก่อนที่จะเพิ่มเนื้อที่ว่างลงในกล่องจดหมายเก็บถาวร ดังนั้น เราขอแนะให้ผู้ดูแลระบบตรวจสอบพื้นที่ว่างในกล่องจดหมายเก็บถาวร ซึ่งช่วยให้ผู้ใช้สามารถใช้กล่องจดหมายเก็บถาวรต่อไปในขณะที่ขยายได้ For more information, see [Overview of unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) Enable unlimited [archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).

For more information on accessing the archive mailbox from Outlook, [see Outlook requirements for accessing items in an auto-expanded archive](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). เมื่อต้องการกําหนดค่านโยบายการเก็บข้อมูลที่จะย้ายรายการไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติ[ให้ดู ตั้งค่านโยบายการเก็บถาวรและการลบกล่องจดหมายในMicrosoft 365องค์กรของคุณ](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)

**หมายเหตุ**: การเก็บถาวรแบบขยายอัตโนมัติไม่ได้รับการสนับสนุนในกล่องจดหมายหลักExchange 2010
