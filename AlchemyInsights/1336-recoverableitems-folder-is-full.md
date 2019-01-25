---
title: 1336 RecoverableItems โฟลเดอร์นั้นเต็ม
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493460"
---
# <a name="the-recoverable-items-folder-is-full"></a>โฟลเดอร์รายการที่ได้รับคืนที่จะเต็ม

สำหรับกล่องจดหมาย Exchange แบบออนไลน์ใน Office 365 เนื้อที่เก็บเริ่มต้นสำหรับโฟลเดอร์ที่ได้รับคืนสินค้าคือ 30 GB เนื้อที่เก็บสำหรับโฟลเดอร์ที่ได้รับคืนสินค้าจะเพิ่มขึ้นเป็น 100 GB โดยอัตโนมัติถ้ากล่องจดหมายที่อยู่ในการดำเนินคดีค้างไว้ หยุด eDiscovery หรือถูกกำหนดให้กับนโยบายการเก็บข้อมูลของ Office 365
  
เมื่อโฟลเดอร์ได้รับคืนสินค้าที่มาถึงขีดจำกัดเก็บข้อมูล ฟังก์ชันการทำงานของกล่องจดหมายได้รับผลกระทบด้วยวิธีการดังต่อไปนี้:
  
- ผู้ใช้ไม่สามารถลบรายการออกจากกล่องจดหมาย
    
- ผู้จัดการโฟลเดอร์ช่วยไม่สามารถลบสินค้าตามแท็กการเก็บข้อมูลหรือการตั้งค่าโฟลเดอร์ที่มีการจัดการ
    
- สำหรับกล่องจดหมายที่มีการกู้คืนรายการเดียวที่เปิดใช้งาน หรือถูกหยุดไว้ กระบวนการป้องกันการคัดลอกเมื่อเขียนหน้าไม่สามารถรักษารุ่นของรายการที่แก้ไข โดยผู้ใช้
    
- สำหรับกล่องจดหมายที่มีกล่องจดหมายที่เปิดใช้งานการล็อกการตรวจสอบ รายการล็อกการตรวจสอบไม่มีกล่องจดหมายที่สามารถบันทึกในการตรวจสอบโฟลเดอร์ย่อยในโฟลเดอร์รายการที่กู้คืน
    
ผู้ดูแลระบบสามารถใช้สำหรับกล่องจดหมายที่ไม่คงค้าง การ`Search-Mailbox -SearchDumpsterOnly -DeleteContent`คำสั่งในการแลกเปลี่ยน PowerShell ออนไลน์เพื่อลบรายการในโฟลเดอร์รายการที่กู้คืนได้ สำหรับข้อมูลเพิ่มเติม ดูหัวข้อต่อไปนี้: 
  
- [ค้นหา และลบข้อความ](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [ค้นหาจดหมาย](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
สำหรับกล่องจดหมายที่คงค้าง มี admins เพื่อลบการระงับก่อนที่จะสามารถมีรายการที่ถูกลบจากโฟลเดอร์รายการที่กู้คืน ดูข้อมูลเพิ่มเติม[ลบรายการในชุดรายการได้รับคืนที่โฟลเดอร์ของกล่องจดหมายที่ใช้ cloud บนค้างไว้](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)
  
เพื่อช่วยป้องกันไม่ให้กลายเป็นทั้งหมดในโฟลเดอร์รายการที่ได้รับคืน admins สามารถเพิ่มขีดจำกัดการเก็บข้อมูลของสินค้าได้รับคืนโฟลเดอร์สำหรับกล่องจดหมายบนค้างไว้ และตั้งค่านโยบายการเก็บข้อมูลกล่องจดหมายที่ย้ายสินค้าจากโฟลเดอร์รายการที่กู้คืนไปที่เก็บถาวรของผู้ใช้ กล่องจดหมาย ดู[เพิ่มโควต้าสำหรับกล่องจดหมายในที่เก็บสินค้าได้รับคืน](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
  

