---
title: โฟลเดอร์ 1336 RecoverableItems เต็ม
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061775"
---
# <a name="the-recoverable-items-folder-is-full"></a>โฟลเดอร์รายการที่กู้คืนได้เต็ม

For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB. ขีดจํากัดของที่เก็บข้อมูลโฟลเดอร์รายการที่กู้คืนได้จะถูกเพิ่มเป็น 100 GB โดยอัตโนมัติถ้ากล่องจดหมายถูกวางไว้ใน Litigation Hold, eDiscovery hold หรือถูกมอบหมายให้กับนโยบายการเก็บข้อมูล

เมื่อโฟลเดอร์รายการที่กู้คืนได้ถึงขีดจํากัดของที่เก็บข้อมูล ฟังก์ชันการโยกย้ายกล่องจดหมายจะได้รับผลกระทบด้วยวิธีต่อไปนี้:

- ผู้ใช้ไม่สามารถลบรายการจากกล่องจดหมายได้

- ตัวช่วยโฟลเดอร์ที่มีการจัดการไม่สามารถลบรายการตามแท็กการเก็บข้อมูลหรือการตั้งค่าโฟลเดอร์ที่มีการจัดการ

- For mailboxes that have Single Item Recovery enabled or are placed hold, the copy-on-write page protection process can't maintain versions of items edited by the user.

- For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits folder in the Recoverable Items folder.

For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. ดูข้อมูลเพิ่มเติมที่หัวข้อต่อไปนี้:

- [ค้นหาและลบข้อความ](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

เพื่อช่วยป้องกันไม่ให้โฟลเดอร์รายการที่กู้คืนได้เต็ม ผู้ดูแลระบบสามารถเพิ่มขีดจํากัดที่เก็บข้อมูลของโฟลเดอร์รายการที่กู้คืนได้ระงับกล่องจดหมาย และตั้งค่านโยบายการเก็บข้อมูลกล่องจดหมายที่ย้ายรายการจากโฟลเดอร์รายการที่กู้คืนได้ไปยังกล่องจดหมายเก็บถาวรของผู้ใช้ ให้ดูที่[เพิ่มโควตารายการที่กู้คืนได้ระงับกล่องจดหมาย](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
