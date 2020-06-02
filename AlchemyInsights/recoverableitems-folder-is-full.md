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
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="448c3-102">โฟลเดอร์รายการที่สามารถกู้คืนได้เต็ม</span><span class="sxs-lookup"><span data-stu-id="448c3-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="448c3-103">สําหรับกล่องจดหมาย Exchange แบบออนไลน์ ขีดจํากัดการจัดเก็บเริ่มต้นสําหรับโฟลเดอร์รายการกู้คืนได้คือ 30 GB</span><span class="sxs-lookup"><span data-stu-id="448c3-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="448c3-104">ขีดจํากัดการจัดเก็บสําหรับโฟลเดอร์รายการที่ได้รับคืนจะเพิ่มขึ้นโดยอัตโนมัติเป็น 100 GB ถ้ากล่องจดหมายถูกวางบนการดําเนินคดี Hold eDiscovery หรือถูกกําหนดให้กับนโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="448c3-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="448c3-105">เมื่อโฟลเดอร์รายการที่ได้รับคืนถึงขีดจํากัดการจัดเก็บ</span><span class="sxs-lookup"><span data-stu-id="448c3-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="448c3-106">ผู้ใช้ไม่สามารถลบรายการออกจากกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="448c3-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="448c3-107">ตัวช่วยโฟลเดอร์ที่มีการจัดการไม่สามารถลบรายการตามแท็กการเก็บรักษาหรือการตั้งค่าโฟลเดอร์ที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="448c3-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="448c3-108">สําหรับกล่องจดหมายที่มีการกู้คืนรายการเดียวเปิดใช้งาน หรือถูกพักไว้</span><span class="sxs-lookup"><span data-stu-id="448c3-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="448c3-109">สําหรับกล่องจดหมายที่มีกล่องจดหมายการตรวจสอบล็อกการเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="448c3-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="448c3-110">สําหรับกล่องจดหมายที่ไม่ได้หยุด `Search-Mailbox -SearchDumpsterOnly -DeleteContent`</span><span class="sxs-lookup"><span data-stu-id="448c3-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="448c3-111">สําหรับข้อมูลเพิ่มเติม ให้ดูหัวข้อต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="448c3-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="448c3-112">ค้นหาและลบข้อความ</span><span class="sxs-lookup"><span data-stu-id="448c3-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="448c3-113">ค้นหากล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="448c3-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="448c3-114">สําหรับกล่องจดหมายที่ค้าง</span><span class="sxs-lookup"><span data-stu-id="448c3-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="448c3-115">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ลบรายการในโฟลเดอร์ รายการกู้คืนของกล่องจดหมาย Cloud-Based ที่ค้างอยู่](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)</span><span class="sxs-lookup"><span data-stu-id="448c3-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="448c3-116">เพื่อช่วยป้องกันไม่ให้โฟลเดอร์รายการที่ได้รับคืนจากกลายเป็นแบบเต็ม</span><span class="sxs-lookup"><span data-stu-id="448c3-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="448c3-117">ดู[เพิ่มโควตารายการที่ได้รับคืนสําหรับกล่องจดหมายที่ค้างอยู่](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)</span><span class="sxs-lookup"><span data-stu-id="448c3-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
