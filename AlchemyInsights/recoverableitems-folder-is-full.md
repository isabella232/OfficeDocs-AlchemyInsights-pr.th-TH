---
title: โฟลเดอร์๑๓๓๖ RecoverableItems เต็ม
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
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741286"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="93b61-102">โฟลเดอร์รายการที่สามารถกู้คืนได้เต็มแล้ว</span><span class="sxs-lookup"><span data-stu-id="93b61-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="93b61-103">สำหรับกล่องจดหมาย Exchange Online ขีดจำกัดที่เก็บข้อมูลเริ่มต้นสำหรับโฟลเดอร์รายการที่สามารถกู้คืนได้คือ 30 GB</span><span class="sxs-lookup"><span data-stu-id="93b61-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="93b61-104">ขีดจำกัดของที่เก็บข้อมูลสำหรับโฟลเดอร์รายการที่สามารถกู้คืนได้จะเพิ่มโดยอัตโนมัติไปยัง๑๐๐ GB ถ้ากล่องจดหมายถูกวางไว้บนการระงับการดำเนินคดีการระงับ eDiscovery หรือถูกกำหนดให้กับนโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="93b61-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="93b61-105">เมื่อโฟลเดอร์รายการที่สามารถกู้คืนมาถึงขีดจำกัดที่เก็บข้อมูลฟังก์ชันการทำงานของกล่องจดหมายจะได้รับผลกระทบด้วยวิธีต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="93b61-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="93b61-106">ผู้ใช้ไม่สามารถลบรายการออกจากกล่องจดหมายได้</span><span class="sxs-lookup"><span data-stu-id="93b61-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="93b61-107">ตัวช่วยสร้างโฟลเดอร์ที่มีการจัดการไม่สามารถลบรายการได้โดยยึดตามแท็กการเก็บข้อมูลหรือการตั้งค่าโฟลเดอร์ที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="93b61-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="93b61-108">สำหรับกล่องจดหมายที่มีการกู้คืนรายการเดียวที่เปิดใช้งานอยู่หรือจะถูกวางไว้บนการระงับการป้องกันหน้าการป้องกันการคัดลอกบนเขียนไม่สามารถรักษาเวอร์ชันของรายการที่แก้ไขโดยผู้ใช้ได้</span><span class="sxs-lookup"><span data-stu-id="93b61-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="93b61-109">สำหรับกล่องจดหมายที่มีการเปิดใช้งานการบันทึกการตรวจสอบของกล่องจดหมายไม่สามารถบันทึกรายการบันทึกการตรวจสอบของกล่องจดหมายในโฟลเดอร์ย่อยการตรวจสอบในโฟลเดอร์รายการที่สามารถกู้คืนได้</span><span class="sxs-lookup"><span data-stu-id="93b61-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="93b61-110">สำหรับกล่องจดหมายที่ไม่ได้ถูกระงับผู้ดูแลระบบสามารถใช้ `Search-Mailbox -SearchDumpsterOnly -DeleteContent` คำสั่งใน PowerShell Online Exchange เพื่อลบรายการในโฟลเดอร์รายการที่สามารถกู้คืนได้</span><span class="sxs-lookup"><span data-stu-id="93b61-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="93b61-111">สำหรับข้อมูลเพิ่มเติมให้ดูหัวข้อต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="93b61-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="93b61-112">ค้นหาและลบข้อความ</span><span class="sxs-lookup"><span data-stu-id="93b61-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="93b61-113">ค้นหา-กล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="93b61-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="93b61-114">สำหรับกล่องจดหมายที่ถูกระงับผู้ดูแลระบบต้องเอาการระงับออกก่อนที่พวกเขาจะสามารถลบรายการจากโฟลเดอร์รายการที่สามารถกู้คืนได้</span><span class="sxs-lookup"><span data-stu-id="93b61-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="93b61-115">สำหรับข้อมูลเพิ่มเติมให้ดู [ลบรายการในโฟลเดอร์รายการที่สามารถกู้คืนของกล่องจดหมายที่ใช้ระบบคลาวด์](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)ได้</span><span class="sxs-lookup"><span data-stu-id="93b61-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="93b61-116">เพื่อช่วยป้องกันไม่ให้โฟลเดอร์รายการที่สามารถกู้คืนได้เป็นแบบเต็มผู้ดูแลระบบสามารถเพิ่มขีดจำกัดของที่เก็บข้อมูลของโฟลเดอร์รายการที่สามารถกู้คืนได้สำหรับกล่องจดหมายที่ระงับและตั้งค่านโยบายการเก็บข้อมูลของกล่องจดหมายที่ย้ายรายการจากโฟลเดอร์รายการที่สามารถกู้คืนไปยังกล่องจดหมายเก็บถาวรของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="93b61-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="93b61-117">ดู[เพิ่มโควตาของรายการที่สามารถกู้คืนสำหรับกล่องจดหมายที่ถูกระงับ](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)</span><span class="sxs-lookup"><span data-stu-id="93b61-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
