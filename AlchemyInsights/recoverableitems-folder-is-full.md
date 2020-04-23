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
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="5dd62-102">โฟลเดอร์รายการได้รับคืนเต็ม</span><span class="sxs-lookup"><span data-stu-id="5dd62-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="5dd62-103">สําหรับกล่องจดหมาย Exchange แบบออนไลน์ ขีดจํากัดการจัดเก็บเริ่มต้นสําหรับโฟลเดอร์รายการกู้คืนคือ 30 กิกะไบต์</span><span class="sxs-lookup"><span data-stu-id="5dd62-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="5dd62-104">ขีดจํากัดการจัดเก็บสําหรับโฟลเดอร์รายการที่ได้รับคืนจะเพิ่มขึ้นโดยอัตโนมัติเป็น 100 กิกะไบต์ถ้ากล่องจดหมายถูกวางไว้บน Litigation Hold, eDiscovery ระงับ หรือถูกกําหนดให้กับนโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="5dd62-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="5dd62-105">เมื่อโฟลเดอร์รายการที่ได้รับคืนถึงขีดจํากัดการจัดเก็บ ฟังก์ชันการทํางานของกล่องจดหมายได้รับผลกระทบในลักษณะต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="5dd62-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="5dd62-106">ผู้ใช้ไม่สามารถลบรายการจากกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="5dd62-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="5dd62-107">ผู้ช่วยโฟลเดอร์ที่มีการจัดการไม่สามารถลบรายการตามแท็กการเก็บรักษาหรือการตั้งค่าโฟลเดอร์ที่มีการจัดการได้</span><span class="sxs-lookup"><span data-stu-id="5dd62-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="5dd62-108">สําหรับกล่องจดหมายที่มีการเปิดใช้งานการกู้คืนรายการเดียวหรือถูกพักไว้</span><span class="sxs-lookup"><span data-stu-id="5dd62-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="5dd62-109">สําหรับกล่องจดหมายที่มีการเปิดใช้งานการบันทึกการตรวจสอบกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="5dd62-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="5dd62-110">สําหรับกล่องจดหมายที่ไม่หยุด admins สามารถใช้`Search-Mailbox -SearchDumpsterOnly -DeleteContent`คําสั่งใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนเมื่อต้องการลบรายการในโฟลเดอร์รายการที่ได้รับคืน</span><span class="sxs-lookup"><span data-stu-id="5dd62-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="5dd62-111">สําหรับข้อมูลเพิ่มเติม ให้ดูหัวข้อต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="5dd62-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="5dd62-112">ค้นหาและลบข้อความ</span><span class="sxs-lookup"><span data-stu-id="5dd62-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="5dd62-113">ค้นหากล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="5dd62-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="5dd62-114">สําหรับกล่องจดหมายที่หยุดไว้</span><span class="sxs-lookup"><span data-stu-id="5dd62-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="5dd62-115">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การลบรายการในโฟลเดอร์ รายการที่สามารถกู้คืนได้ ของกล่องจดหมาย Cloud-Based ที่หยุดไว้](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)</span><span class="sxs-lookup"><span data-stu-id="5dd62-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="5dd62-116">เพื่อช่วยป้องกันไม่ให้โฟลเดอร์รายการที่ได้รับคืนจากกลายเป็นแบบเต็ม admins สามารถเพิ่มขีดจํากัดการจัดเก็บของโฟลเดอร์รายการคืนสําหรับกล่องจดหมายที่ระงับ และตั้งค่านโยบายการเก็บข้อมูลกล่องจดหมายที่ย้ายรายการจากโฟลเดอร์รายการที่กู้คืนไปยังกล่องจดหมายเก็บถาวรของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="5dd62-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="5dd62-117">ดูที่[เพิ่มโควตารายการรับคืนสําหรับกล่องจดหมายที่หยุดไว้](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)</span><span class="sxs-lookup"><span data-stu-id="5dd62-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
