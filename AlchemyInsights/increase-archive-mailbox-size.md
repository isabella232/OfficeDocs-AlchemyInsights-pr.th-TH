---
title: 305 เพิ่มขนาดกล่องจดหมายเก็บถาวร
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 28086145d8769bd06ef6352257a820146c5f237d
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391585"
---
# <a name="increase-the-archive-mailbox-size"></a><span data-ttu-id="688a6-102">เพิ่มขนาดกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="688a6-102">Increase the archive mailbox size</span></span>

<span data-ttu-id="688a6-103">Office 365[ขีดจำกัด](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)ขนาดของกล่องจดหมายที่เก็บถาวรที่ขึ้นอยู่กับสิทธิ์การใช้งานที่ถูกกำหนดให้กับบัญชีผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="688a6-103">Office 365 [limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) the size of archive mailboxes based on the license that's assigned to the user account.</span></span> <span data-ttu-id="688a6-104">เมื่อกล่องจดหมายเก็บถาวรถึง 90% ของขนาดที่ใช้ได้ ผู้ใช้ได้รับการแจ้งเตือนทางอีเมล</span><span class="sxs-lookup"><span data-stu-id="688a6-104">When the archive mailbox reaches 90% of its allowed size, the user receives an email notification.</span></span> <span data-ttu-id="688a6-105">เมื่อกล่องจดหมายการเก็บถาวรได้ถึงขีดจำกัดของขนาด ผู้ใช้ไม่สามารถย้ายรายการไปยังกล่องจดหมายการเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="688a6-105">When an archive mailbox reaches its size limit, the user can't move more items to the archive mailbox.</span></span> <span data-ttu-id="688a6-106">Office 365 จะไม่เพิ่มขนาดของกล่องจดหมายเก็บถาวรเมื่อถึงขนาดจำกัดไว้</span><span class="sxs-lookup"><span data-stu-id="688a6-106">Office 365 won't increase the size of an archive mailbox once the size limit is reached.</span></span> <span data-ttu-id="688a6-107">แทน ผู้ใช้สามารถดำเนินการดังต่อไปนี้เพื่อเพิ่มเนื้อที่ในการเก็บถาวรกล่องจดหมาย:</span><span class="sxs-lookup"><span data-stu-id="688a6-107">Instead, users can take the following actions to free up space in the archive mailbox:</span></span>

- <span data-ttu-id="688a6-108">ส่งออกรายการไปยังแฟ้ม.pst โดยใช้ Outlook</span><span class="sxs-lookup"><span data-stu-id="688a6-108">Export the the items to a .pst file using Outlook</span></span>

- <span data-ttu-id="688a6-109">ลบรายการออกจากกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="688a6-109">Delete items from the archive mailbox.</span></span>

<span data-ttu-id="688a6-110">Office 365 ให้**เก็บถาวรไม่จำกัด**สำหรับใบอนุญาต E3 องค์กร 365 Office และ E5</span><span class="sxs-lookup"><span data-stu-id="688a6-110">Office 365 provides **unlimited archiving** for Office 365 Enterprise E3 and E5 licenses.</span></span> <span data-ttu-id="688a6-111">Admin ต้องเปิดใช้งานคุณลักษณะนี้ก่อนที่เก็บกล่องจดหมายมาถึงขนาดสูงสุด</span><span class="sxs-lookup"><span data-stu-id="688a6-111">An admin must enable this feature before the archive mailbox reaches its maximum size.</span></span> <span data-ttu-id="688a6-112">เมื่อมีการใช้การเก็บถาวรไม่จำกัด ซึ่งอาจใช้เวลาถึง 30 วันก่อนช่องว่างถูกเพิ่มไปยังกล่องจดหมายการเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="688a6-112">When unlimited archiving is enabled, it can take up to 30 days before free space is added to the archive mailbox.</span></span> <span data-ttu-id="688a6-113">ดังนั้น เราขอแนะนำให้ ผู้ดูแลตรวจสอบเนื้อที่ว่างในการเก็บถาวรกล่องจดหมาย ซึ่งช่วยให้ผู้ใช้ใช้กล่องจดหมายการเก็บถาวรในขณะนั้นขยายต่อไป</span><span class="sxs-lookup"><span data-stu-id="688a6-113">Therefore, we recommend that admins verify the free space in the archive mailbox, which allows the user to continue using the archive mailbox while it expands.</span></span> <span data-ttu-id="688a6-114">สำหรับข้อมูลเพิ่มเติม ดู[ภาพรวมของการเก็บถาวรใน Office 365 ไม่จำกัด](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving)และการ[เปิดใช้งานการเก็บถาวรได้ไม่จำกัดใน Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving)</span><span class="sxs-lookup"><span data-stu-id="688a6-114">For more information, see [Overview of unlimited archiving in Office 365](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) and [Enable unlimited archiving in Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving).</span></span>

<span data-ttu-id="688a6-115">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเข้าถึงกล่องจดหมายเก็บถาวรจาก Outlook ดู[ความต้องการของ Outlook สำหรับการเข้าถึงรายการในเก็บถาวรอัตโนมัติถูกขยาย](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)</span><span class="sxs-lookup"><span data-stu-id="688a6-115">For more information on accessing the archive mailbox from Outlook, see [Outlook requirements for accessing items in an auto-expanded archive](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive).</span></span> <span data-ttu-id="688a6-116">เมื่อต้องการกำหนดค่านโยบายการเก็บข้อมูลที่ย้ายรายการไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติ ดู[การตั้งค่านโยบายการเก็บถาวรและการลบสำหรับกล่องจดหมายในองค์กรของคุณ Office 365](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="688a6-116">To configure a retention policy that automatically moves items to the archive mailbox, see [Set up an archive and deletion policy for mailboxes in your Office 365 organization](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).</span></span>

<span data-ttu-id="688a6-117">**หมายเหตุ**: แฟ้มเก็บถาวรที่ขยายได้อัตโนมัติไม่ได้รับการสนับสนุนสำหรับกล่องจดหมายหลักบน Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="688a6-117">**Note**: Auto-expanding archives aren't supported for primary mailboxes on Exchange 2010.</span></span>
