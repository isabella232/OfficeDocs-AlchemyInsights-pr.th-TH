---
title: โฟลเดอร์ 1336 กู้คืนรายการเต็ม
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720271"
---
# <a name="the-recoverable-items-folder-is-full"></a>โฟลเดอร์รายการได้รับคืนเต็ม

สําหรับกล่องจดหมาย Exchange แบบออนไลน์ ขีดจํากัดการจัดเก็บเริ่มต้นสําหรับโฟลเดอร์รายการกู้คืนคือ 30 กิกะไบต์ ขีดจํากัดการจัดเก็บสําหรับโฟลเดอร์รายการที่ได้รับคืนจะเพิ่มขึ้นโดยอัตโนมัติเป็น 100 กิกะไบต์ถ้ากล่องจดหมายถูกวางไว้บน Litigation Hold, eDiscovery ระงับ หรือถูกกําหนดให้กับนโยบายการเก็บข้อมูล

เมื่อโฟลเดอร์รายการที่ได้รับคืนถึงขีดจํากัดการจัดเก็บ ฟังก์ชันการทํางานของกล่องจดหมายได้รับผลกระทบในลักษณะต่อไปนี้:

- ผู้ใช้ไม่สามารถลบรายการจากกล่องจดหมาย

- ผู้ช่วยโฟลเดอร์ที่มีการจัดการไม่สามารถลบรายการตามแท็กการเก็บรักษาหรือการตั้งค่าโฟลเดอร์ที่มีการจัดการได้

- สําหรับกล่องจดหมายที่มีการเปิดใช้งานการกู้คืนรายการเดียวหรือถูกพักไว้

- สําหรับกล่องจดหมายที่มีการเปิดใช้งานการบันทึกการตรวจสอบกล่องจดหมาย

สําหรับกล่องจดหมายที่ไม่หยุด admins สามารถใช้`Search-Mailbox -SearchDumpsterOnly -DeleteContent`คําสั่งใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนเมื่อต้องการลบรายการในโฟลเดอร์รายการที่ได้รับคืน สําหรับข้อมูลเพิ่มเติม ให้ดูหัวข้อต่อไปนี้:

- [ค้นหาและลบข้อความ](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [ค้นหากล่องจดหมาย](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

สําหรับกล่องจดหมายที่หยุดไว้ สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การลบรายการในโฟลเดอร์ รายการที่สามารถกู้คืนได้ ของกล่องจดหมาย Cloud-Based ที่หยุดไว้](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

เพื่อช่วยป้องกันไม่ให้โฟลเดอร์รายการที่ได้รับคืนจากกลายเป็นแบบเต็ม admins สามารถเพิ่มขีดจํากัดการจัดเก็บของโฟลเดอร์รายการคืนสําหรับกล่องจดหมายที่ระงับ และตั้งค่านโยบายการเก็บข้อมูลกล่องจดหมายที่ย้ายรายการจากโฟลเดอร์รายการที่กู้คืนไปยังกล่องจดหมายเก็บถาวรของผู้ใช้ ดูที่[เพิ่มโควตารายการรับคืนสําหรับกล่องจดหมายที่หยุดไว้](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
