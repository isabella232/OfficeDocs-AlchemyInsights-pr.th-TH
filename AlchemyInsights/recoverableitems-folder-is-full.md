---
title: 1336 RecoverableItems โฟลเดอร์เต็ม
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
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510771"
---
# <a name="the-recoverable-items-folder-is-full"></a>โฟลเดอร์รายการที่สามารถกู้คืนได้เต็ม

สําหรับกล่องจดหมาย Exchange แบบออนไลน์ ขีดจํากัดการจัดเก็บเริ่มต้นสําหรับโฟลเดอร์รายการกู้คืนได้คือ 30 GB ขีดจํากัดการจัดเก็บสําหรับโฟลเดอร์รายการที่ได้รับคืนจะเพิ่มขึ้นโดยอัตโนมัติเป็น 100 GB ถ้ากล่องจดหมายถูกวางบนการดําเนินคดี Hold eDiscovery หรือถูกกําหนดให้กับนโยบายการเก็บข้อมูล

เมื่อโฟลเดอร์รายการที่ได้รับคืนถึงขีดจํากัดการจัดเก็บ

- ผู้ใช้ไม่สามารถลบรายการออกจากกล่องจดหมาย

- ตัวช่วยโฟลเดอร์ที่มีการจัดการไม่สามารถลบรายการตามแท็กการเก็บรักษาหรือการตั้งค่าโฟลเดอร์ที่มีการจัดการ

- สําหรับกล่องจดหมายที่มีการกู้คืนรายการเดียวเปิดใช้งาน หรือถูกพักไว้

- สําหรับกล่องจดหมายที่มีกล่องจดหมายการตรวจสอบล็อกการเปิดใช้งาน

สําหรับกล่องจดหมายที่ไม่ได้หยุด `Search-Mailbox -SearchDumpsterOnly -DeleteContent` สําหรับข้อมูลเพิ่มเติม ให้ดูหัวข้อต่อไปนี้:

- [ค้นหาและลบข้อความ](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [ค้นหากล่องจดหมาย](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

สําหรับกล่องจดหมายที่ค้าง สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ลบรายการในโฟลเดอร์ รายการกู้คืนของกล่องจดหมาย Cloud-Based ที่ค้างอยู่](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

เพื่อช่วยป้องกันไม่ให้โฟลเดอร์รายการที่ได้รับคืนจากกลายเป็นแบบเต็ม ดู[เพิ่มโควตารายการที่ได้รับคืนสําหรับกล่องจดหมายที่ค้างอยู่](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
