---
title: การแก้ไขปัญหา Microsoft Defender สำหรับ Office ๓๖๕
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801465"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>การแก้ไขปัญหา Microsoft Defender สำหรับ Office ๓๖๕

- คุณสังเกตเห็นความล่าช้าในการนำส่งข้อความหรือไม่ ใช้ตัวเลือกการนำ [ส่งแบบไดนามิก](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) ในนโยบายสิ่งที่แนบมาของ ATP Safe ของคุณ การทำเช่นนี้จะช่วยหลีกเลี่ยงความล่าช้าของข้อความในขณะที่ปกป้องผู้รับจากไฟล์ที่เป็นอันตราย

- คุณต้องการรายงาน false บวกหรือค่าลบ false ไปยังไมโครซอฟท์หรือไม่ ใช้ [ลิงก์](https://www.microsoft.com/wdsi/filesubmission/) นี้เพื่อส่งไฟล์สำหรับการวิเคราะห์

- คุณทราบหรือไม่ว่าคุณสามารถเปิดใช้งานการป้องกันลิงก์ที่ปลอดภัยสำหรับอีเมลภายในที่ส่งระหว่างผู้รับภายในองค์กรของคุณได้ ให้ทำตามขั้นตอนต่อไปนี้:

  1. ไปที่ [https://protection.office.com](https://protection.office.com) แล้วลงชื่อเข้าใช้ด้วยบัญชีผู้ดูแลระบบส่วนกลางหรือบัญชีผู้ดูแลระบบความปลอดภัย

  2. ในบานหน้าต่างนำทางด้านซ้ายภายใต้ **การจัดการภัยคุกคาม** ให้เลือก **Policy** \> **ลิงก์ที่ปลอดภัย** ตามนโยบาย

  3. ใน **นโยบายที่นำไปใช้กับส่วนทั้งหมดขององค์กร** ให้เลือกนโยบายแล้วคลิก **แก้ไข**

  4. ภายใต้ **การตั้งค่า** ให้เปิดใช้งาน **ลิงก์ที่ปลอดภัยไปยังข้อความที่ส่งภายในองค์กร**
