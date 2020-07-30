---
title: 305เพิ่มขนาดกล่องจดหมายเก็บถาวร
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: c43f8e32acad7937a03a45aab1e14e0e69edc1b2
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522862"
---
# <a name="increase-the-archive-mailbox-size"></a>เพิ่มขนาดกล่องจดหมายเก็บถาวร


หากคุณต้องการให้เราเรียกใช้การตรวจสอบอัตโนมัติสําหรับการตั้งค่าที่กล่าวถึงด้านล่างให้เลือกปุ่มย้อนกลับ< -- ที่ด้านบนของหน้านี้แล้วป้อนที่อยู่อีเมลของผู้ใช้ที่ต้องการขนาดกล่องจดหมายของพวกเขาเก็บถาวรเพิ่มขึ้น

Microsoft 365[จํากัด](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)ขนาดของกล่องจดหมายเก็บถาวรตามสิทธิ์การใช้งานที่กําหนดให้กับบัญชีผู้ใช้ เมื่อกล่องจดหมายเก็บถาวรถึง 90% ของขนาดที่ได้รับอนุญาต เมื่อกล่องจดหมายเก็บถาวรถึงขนาดจํากัดผู้ใช้ไม่สามารถย้ายรายการเพิ่มเติมไปยังกล่องจดหมายเก็บถาวร Microsoft 365 จะไม่เพิ่มขนาดของกล่องจดหมายเก็บถาวรเมื่อถึงขีดจํากัดขนาด ผู้ใช้สามารถดําเนินการต่อไปนี้เพื่อเพิ่มพื้นที่ว่างในกล่องจดหมายเก็บถาวรแทน:

- ส่งออกรายการไปยังแฟ้ม .pst โดยใช้ Outlook

- ลบรายการออกจากกล่องจดหมายเก็บถาวร

Microsoft 365 ให้**ไม่จํากัดเก็บ**สําหรับ Office 365 E3 องค์กร E3 และ E5 สิทธิ์การใช้งาน ผู้ดูแลต้องเปิดใช้งานคุณลักษณะนี้ก่อนที่กล่องจดหมายเก็บถาวรถึงขนาดสูงสุด เมื่อเปิดใช้งานการเก็บถาวรแบบไม่จํากัด อาจใช้เวลาถึง 30 วันก่อนที่การเพิ่มเนื้อที่ว่างลงในกล่องจดหมายเก็บถาวร ดังนั้น เราขอแนะนําให้ผู้ดูแลระบบตรวจสอบพื้นที่ว่างในกล่องจดหมายเก็บถาวร ซึ่งช่วยให้ผู้ใช้สามารถใช้กล่องจดหมายเก็บถาวรต่อไปในขณะที่ขยาย สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ภาพรวมของการเก็บถาวรแบบไม่จํากัดใน Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving)และ[เปิดใช้งานการเก็บถาวรแบบไม่จํากัดใน Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving)

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการเข้าถึงกล่องจดหมายเก็บถาวรจาก Outlook ให้ดูที่[ข้อกําหนดของ Outlook สําหรับการเข้าถึงรายการในที่เก็บถาวรที่ขยายอัตโนมัติ](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive) เมื่อต้องการกําหนดค่านโยบายการเก็บข้อมูลที่ย้ายรายการไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติ ให้ดูที่[การตั้งค่านโยบายการเก็บถาวรและการลบสําหรับกล่องจดหมายในองค์กรของคุณ Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)

**หมายเหตุ**: เก็บถาวรที่ขยายอัตโนมัติไม่ได้รับการสนับสนุนสําหรับกล่องจดหมายหลักบน Exchange 2010
