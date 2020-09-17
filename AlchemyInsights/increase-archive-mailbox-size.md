---
title: ๓๐๕เพิ่มขนาดกล่องจดหมายเก็บถาวร
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
ms.openlocfilehash: 6bebc17eafd8615a6ffa95dbdf16f60768204aa7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778602"
---
# <a name="increase-the-archive-mailbox-size"></a>เพิ่มขนาดกล่องจดหมายเก็บถาวร


ถ้าคุณต้องการให้เราเรียกใช้การตรวจสอบโดยอัตโนมัติสำหรับการตั้งค่าที่ระบุไว้ด้านล่างให้เลือกปุ่มย้อนกลับ <-ที่ด้านบนสุดของหน้านี้แล้วใส่ที่อยู่อีเมลของผู้ใช้ที่ต้องการเพิ่มขนาดของกล่องจดหมายเก็บถาวร

Microsoft ๓๖๕ [จำกัด](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) ขนาดของกล่องจดหมายเก็บถาวรโดยยึดตามสิทธิ์การใช้งานที่ได้รับมอบหมายให้กับบัญชีผู้ใช้ เมื่อกล่องจดหมายเก็บถาวรถึง๙๐% ของขนาดที่อนุญาตผู้ใช้จะได้รับการแจ้งให้ทราบทางอีเมล เมื่อกล่องจดหมายเก็บถาวรถึงขีดจำกัดของขนาดผู้ใช้ไม่สามารถย้ายรายการเพิ่มเติมไปยังกล่องจดหมายเก็บถาวรได้ Microsoft ๓๖๕จะไม่เพิ่มขนาดของกล่องจดหมายเก็บถาวรเมื่อถึงขีดจำกัดขนาด แต่ผู้ใช้สามารถดำเนินการต่อไปนี้เพื่อเพิ่มพื้นที่ว่างในกล่องจดหมายเก็บถาวรดังต่อไปนี้

- ส่งออกรายการไปยังไฟล์ .pst โดยใช้ Outlook

- ลบรายการออกจากกล่องจดหมายเก็บถาวร

Microsoft ๓๖๕มีการ **เก็บถาวรแบบไม่จำกัด** สำหรับ Office ๓๖๕ Enterprise E3 และ E5 สิทธิ์การใช้งาน ผู้ดูแลระบบต้องเปิดใช้งานฟีเจอร์นี้ก่อนที่กล่องจดหมายเก็บถาวรจะมาถึงขนาดสูงสุด เมื่อเปิดใช้งานการเก็บถาวรแบบไม่จำกัดอาจใช้เวลาถึง30วันก่อนที่จะเพิ่มเนื้อที่ว่างลงในกล่องจดหมายเก็บถาวร ดังนั้นเราจึงขอแนะนำให้ผู้ดูแลระบบตรวจสอบพื้นที่ว่างในกล่องจดหมายเก็บถาวรซึ่งจะช่วยให้ผู้ใช้สามารถใช้กล่องจดหมายเก็บถาวรต่อไปได้ในขณะที่มีการขยาย สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ภาพรวมของการเก็บถาวรแบบไม่จำกัดใน microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving)และ[เปิดใช้งานการเก็บถาวรแบบไม่จำกัดใน microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเข้าถึงกล่องจดหมายเก็บถาวรจาก Outlook ให้ดู[ที่ความต้องการของ outlook สำหรับการเข้าถึงรายการในที่เก็บถาวรที่ขยายอัตโนมัติ](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive) เมื่อต้องการกำหนดค่านโยบายการเก็บข้อมูลที่จะย้ายรายการไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติให้ดูที่[ตั้งค่านโยบายการเก็บถาวรและการลบสำหรับกล่องจดหมายในองค์กร Microsoft ๓๖๕ของคุณ](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)

**หมายเหตุ**: ที่เก็บถาวรที่ขยายอัตโนมัติไม่ได้รับการสนับสนุนสำหรับกล่องจดหมายหลักบน Exchange ๒๐๑๐
