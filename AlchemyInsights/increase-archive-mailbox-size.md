---
title: ๓๐๕เพิ่มขนาดกล่องจดหมายเก็บถาวร
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: a8c16d97040e9396d6cf9bd4a5da671a7da88e13
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/15/2019
ms.locfileid: "36661819"
---
# <a name="increase-the-archive-mailbox-size"></a>เพิ่มขนาดกล่องจดหมายเก็บถาวร

Office ๓๖๕[จำกัด](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)ขนาดของกล่องจดหมายเก็บถาวรตามใบอนุญาตที่กำหนดให้กับบัญชีผู้ใช้ เมื่อกล่องจดหมายเก็บถาวรถึง๙๐% ของขนาดที่อนุญาตผู้ใช้ได้รับการแจ้งเตือนทางเมล เมื่อกล่องจดหมายเก็บถาวรถึงขีดจำกัดขนาดผู้ใช้ไม่สามารถย้ายรายการเพิ่มเติมไปยังกล่องจดหมายเก็บถาวร Office ๓๖๕จะไม่เพิ่มขนาดของกล่องจดหมายเก็บถาวรเมื่อถึงขีดจำกัดขนาด แต่ผู้ใช้สามารถทำการดำเนินการต่อไปนี้เพื่อเพิ่มเนื้อที่ว่างในกล่องจดหมายเก็บถาวร:

- ส่งออกรายการไปยังแฟ้ม. pst โดยใช้ Outlook

- ลบรายการออกจากกล่องจดหมายเก็บถาวร

Office ๓๖๕มีการ**เก็บถาวรแบบไม่จำกัด**สำหรับ Office ๓๖๕องค์กร E3 และสิทธิ์การใช้งาน E5 ผู้ดูแลต้องเปิดใช้งานคุณลักษณะนี้ก่อนกล่องจดหมายเก็บถาวรถึงขนาดสูงสุด เมื่อเปิดใช้งานการเก็บถาวรแบบไม่จำกัดอาจใช้เวลาถึง30วันก่อนที่เนื้อที่ว่างจะถูกเพิ่มลงในกล่องจดหมายเก็บถาวร ดังนั้นเราขอแนะนำให้ผู้ดูแลระบบตรวจสอบพื้นที่ว่างในกล่องจดหมายเก็บถาวรซึ่งช่วยให้ผู้ใช้สามารถดำเนินการต่อโดยใช้กล่องจดหมายเก็บถาวรในขณะที่จะขยาย สำหรับข้อมูลเพิ่มเติมให้ดู[ภาพรวมของการเก็บถาวรแบบไม่จำกัดใน office ๓๖๕](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving)และ[เปิดใช้งานการเก็บถาวรแบบไม่จำกัดใน office ๓๖๕](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเข้าถึงกล่องจดหมายเก็บถาวรจาก Outlook ดู[ความต้องการของ outlook สำหรับการเข้าถึงรายการในที่เก็บถาวรแบบขยายโดยอัตโนมัติ](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive) ในการกำหนดค่านโยบายการเก็บข้อมูลที่ย้ายรายการไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติให้ดูที่[ตั้งค่านโยบายการเก็บถาวรและการลบสำหรับกล่องจดหมายในองค์กร๓๖๕ของคุณ](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)

**หมายเหตุ**: การขยายอัตโนมัติที่เก็บถาวรไม่ได้รับการสนับสนุนสำหรับกล่องจดหมายหลักบน Exchange ๒๐๑๐
