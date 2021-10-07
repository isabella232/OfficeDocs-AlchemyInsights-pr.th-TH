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
ms.custom:
- "305"
- "7494"
- "3100006"
ms.assetid: ''
ms.openlocfilehash: d74a1baa02a74c8efd3be75ed711a2e994b9b552
ms.sourcegitcommit: 68b50235d10ebb92b594ac3224c55cf0e8452ac9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/07/2021
ms.locfileid: "60226111"
---
# <a name="increase-the-archive-mailbox-size"></a>เพิ่มขนาดกล่องจดหมายเก็บถาวร

Microsoft 365จํากัดขนาดของกล่องจดหมายเก็บถาวรโดยยึดตามสิทธิ์การใช้งานที่มอบหมายให้กับบัญชีผู้ใช้ ผู้ใช้จะได้รับการแจ้งเตือนทางอีเมลเมื่อกล่องจดหมายเก็บถาวรมีขนาดที่อนุญาตถึง 90%

เมื่อกล่องจดหมายเก็บถาวรถึงขีดจํากัดขนาดแล้ว ผู้ใช้ไม่สามารถย้ายรายการเพิ่มเติมไปยังกล่องจดหมายเก็บถาวรได้ Microsoft 365ขนาดกล่องจดหมายเก็บถาวรเมื่อถึงขีดจํากัดขนาดแล้ว แต่ผู้ใช้สามารถจัดการได้ดังต่อไปนี้เพื่อให้มีพื้นที่ว่างในกล่องจดหมายเก็บถาวร:

- ส่งออกรายการเป็นไฟล์ .pst โดยใช้Outlook
- ลบรายการออกจากกล่องจดหมายเก็บถาวร

อย่างไรก็ตาม Microsoft 365ให้การเก็บถาวรแบบขยายโดยอัตโนมัติOffice 365 Enterprise E3 และ E5 ต้องเปิดใช้งานก่อนกล่องจดหมายเก็บถาวรถึงขนาดสูงสุด เมื่อเปิดใช้งานการเก็บถาวรแบบขยายอัตโนมัติ อาจใช้เวลาถึง 30 วันก่อนที่จะเพิ่มพื้นที่ว่างลงในกล่องจดหมายเก็บถาวร

For more information, see [Overview of auto-expanding archiving](https://docs.microsoft.com/microsoft-365/compliance/autoexpanding-archiving) and [Enable auto-expanding archiving - Admin Help](https://docs.microsoft.com/microsoft-365/compliance/enable-autoexpanding-archiving).

For information about accessing the archive with Outlook, see [Outlook requirements for accessing items in an auto-expanded archive](https://docs.microsoft.com/microsoft-365/compliance/autoexpanding-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive).

For information about configuring a retention policy that moves items automatically to the archive mailbox, see [Set up an archive and deletion policy for mailboxes in your Microsoft 365 organization](https://docs.microsoft.com//microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).