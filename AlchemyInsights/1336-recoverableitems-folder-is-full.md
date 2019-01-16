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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28316440"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="4e7c7-102">โฟลเดอร์รายการที่ได้รับคืนที่จะเต็ม</span><span class="sxs-lookup"><span data-stu-id="4e7c7-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="4e7c7-p101">สำหรับกล่องจดหมาย Exchange แบบออนไลน์ใน Office 365 เนื้อที่เก็บเริ่มต้นสำหรับโฟลเดอร์ที่ได้รับคืนสินค้าคือ 30 GB เนื้อที่เก็บสำหรับโฟลเดอร์ที่ได้รับคืนสินค้าจะเพิ่มขึ้นเป็น 100 GB โดยอัตโนมัติถ้ากล่องจดหมายที่อยู่ในการดำเนินคดีค้างไว้ หยุด eDiscovery หรือถูกกำหนดให้กับนโยบายการเก็บข้อมูลของ Office 365</span><span class="sxs-lookup"><span data-stu-id="4e7c7-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="4e7c7-105">เมื่อโฟลเดอร์ได้รับคืนสินค้าที่มาถึงขีดจำกัดเก็บข้อมูล ฟังก์ชันการทำงานของกล่องจดหมายได้รับผลกระทบด้วยวิธีการดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="4e7c7-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="4e7c7-106">ผู้ใช้ไม่สามารถลบรายการออกจากกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="4e7c7-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="4e7c7-107">ผู้จัดการโฟลเดอร์ช่วยไม่สามารถลบสินค้าตามแท็กการเก็บข้อมูลหรือการตั้งค่าโฟลเดอร์ที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="4e7c7-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="4e7c7-108">สำหรับกล่องจดหมายที่มีการกู้คืนรายการเดียวที่เปิดใช้งาน หรือถูกหยุดไว้ กระบวนการป้องกันการคัดลอกเมื่อเขียนหน้าไม่สามารถรักษารุ่นของรายการที่แก้ไข โดยผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="4e7c7-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="4e7c7-109">สำหรับกล่องจดหมายที่มีกล่องจดหมายที่เปิดใช้งานการล็อกการตรวจสอบ รายการล็อกการตรวจสอบไม่มีกล่องจดหมายที่สามารถบันทึกในการตรวจสอบโฟลเดอร์ย่อยในโฟลเดอร์รายการที่กู้คืน</span><span class="sxs-lookup"><span data-stu-id="4e7c7-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="4e7c7-p102">ผู้ดูแลระบบสามารถใช้สำหรับกล่องจดหมายที่ไม่คงค้าง การ`Search-Mailbox -SearchDumpsterOnly -DeleteContent`คำสั่งในการแลกเปลี่ยน PowerShell ออนไลน์เพื่อลบรายการในโฟลเดอร์รายการที่กู้คืนได้ สำหรับข้อมูลเพิ่มเติม ดูหัวข้อต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="4e7c7-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="4e7c7-112">ค้นหา และลบข้อความ</span><span class="sxs-lookup"><span data-stu-id="4e7c7-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="4e7c7-113">ค้นหาจดหมาย</span><span class="sxs-lookup"><span data-stu-id="4e7c7-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="4e7c7-p103">สำหรับกล่องจดหมายที่คงค้าง มี admins เพื่อลบการระงับก่อนที่จะสามารถมีรายการที่ถูกลบจากโฟลเดอร์รายการที่กู้คืน ดูข้อมูลเพิ่มเติม[ลบรายการในชุดรายการได้รับคืนที่โฟลเดอร์ของกล่องจดหมายที่ใช้ cloud บนค้างไว้](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)</span><span class="sxs-lookup"><span data-stu-id="4e7c7-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="4e7c7-p104">เพื่อช่วยป้องกันไม่ให้กลายเป็นทั้งหมดในโฟลเดอร์รายการที่ได้รับคืน admins สามารถเพิ่มขีดจำกัดการเก็บข้อมูลของสินค้าได้รับคืนโฟลเดอร์สำหรับกล่องจดหมายบนค้างไว้ และตั้งค่านโยบายการเก็บข้อมูลกล่องจดหมายที่ย้ายสินค้าจากโฟลเดอร์รายการที่กู้คืนไปที่เก็บถาวรของผู้ใช้ กล่องจดหมาย ดู[เพิ่มโควต้าสำหรับกล่องจดหมายในที่เก็บสินค้าได้รับคืน](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)</span><span class="sxs-lookup"><span data-stu-id="4e7c7-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

