---
title: ๓๐๕เพิ่มขนาดกล่องจดหมายเก็บถาวร
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 6bebc17eafd8615a6ffa95dbdf16f60768204aa7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778602"
---
# <a name="increase-the-archive-mailbox-size"></a><span data-ttu-id="b8cef-102">เพิ่มขนาดกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="b8cef-102">Increase the archive mailbox size</span></span>


<span data-ttu-id="b8cef-103">ถ้าคุณต้องการให้เราเรียกใช้การตรวจสอบโดยอัตโนมัติสำหรับการตั้งค่าที่ระบุไว้ด้านล่างให้เลือกปุ่มย้อนกลับ <-ที่ด้านบนสุดของหน้านี้แล้วใส่ที่อยู่อีเมลของผู้ใช้ที่ต้องการเพิ่มขนาดของกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="b8cef-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who needs their archive mailbox size increased.</span></span>

<span data-ttu-id="b8cef-104">Microsoft ๓๖๕ [จำกัด](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) ขนาดของกล่องจดหมายเก็บถาวรโดยยึดตามสิทธิ์การใช้งานที่ได้รับมอบหมายให้กับบัญชีผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="b8cef-104">Microsoft 365 [limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) the size of archive mailboxes based on the license that's assigned to the user account.</span></span> <span data-ttu-id="b8cef-105">เมื่อกล่องจดหมายเก็บถาวรถึง๙๐% ของขนาดที่อนุญาตผู้ใช้จะได้รับการแจ้งให้ทราบทางอีเมล</span><span class="sxs-lookup"><span data-stu-id="b8cef-105">When the archive mailbox reaches 90% of its allowed size, the user receives an email notification.</span></span> <span data-ttu-id="b8cef-106">เมื่อกล่องจดหมายเก็บถาวรถึงขีดจำกัดของขนาดผู้ใช้ไม่สามารถย้ายรายการเพิ่มเติมไปยังกล่องจดหมายเก็บถาวรได้</span><span class="sxs-lookup"><span data-stu-id="b8cef-106">When an archive mailbox reaches its size limit, the user can't move more items to the archive mailbox.</span></span> <span data-ttu-id="b8cef-107">Microsoft ๓๖๕จะไม่เพิ่มขนาดของกล่องจดหมายเก็บถาวรเมื่อถึงขีดจำกัดขนาด</span><span class="sxs-lookup"><span data-stu-id="b8cef-107">Microsoft 365 won't increase the size of an archive mailbox once the size limit is reached.</span></span> <span data-ttu-id="b8cef-108">แต่ผู้ใช้สามารถดำเนินการต่อไปนี้เพื่อเพิ่มพื้นที่ว่างในกล่องจดหมายเก็บถาวรดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="b8cef-108">Instead, users can take the following actions to free up space in the archive mailbox:</span></span>

- <span data-ttu-id="b8cef-109">ส่งออกรายการไปยังไฟล์ .pst โดยใช้ Outlook</span><span class="sxs-lookup"><span data-stu-id="b8cef-109">Export the the items to a .pst file using Outlook.</span></span>

- <span data-ttu-id="b8cef-110">ลบรายการออกจากกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="b8cef-110">Delete items from the archive mailbox.</span></span>

<span data-ttu-id="b8cef-111">Microsoft ๓๖๕มีการ **เก็บถาวรแบบไม่จำกัด** สำหรับ Office ๓๖๕ Enterprise E3 และ E5 สิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="b8cef-111">Microsoft 365 provides **unlimited archiving** for Office 365 Enterprise E3 and E5 licenses.</span></span> <span data-ttu-id="b8cef-112">ผู้ดูแลระบบต้องเปิดใช้งานฟีเจอร์นี้ก่อนที่กล่องจดหมายเก็บถาวรจะมาถึงขนาดสูงสุด</span><span class="sxs-lookup"><span data-stu-id="b8cef-112">An admin must enable this feature before the archive mailbox reaches its maximum size.</span></span> <span data-ttu-id="b8cef-113">เมื่อเปิดใช้งานการเก็บถาวรแบบไม่จำกัดอาจใช้เวลาถึง30วันก่อนที่จะเพิ่มเนื้อที่ว่างลงในกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="b8cef-113">When unlimited archiving is enabled, it can take up to 30 days before free space is added to the archive mailbox.</span></span> <span data-ttu-id="b8cef-114">ดังนั้นเราจึงขอแนะนำให้ผู้ดูแลระบบตรวจสอบพื้นที่ว่างในกล่องจดหมายเก็บถาวรซึ่งจะช่วยให้ผู้ใช้สามารถใช้กล่องจดหมายเก็บถาวรต่อไปได้ในขณะที่มีการขยาย</span><span class="sxs-lookup"><span data-stu-id="b8cef-114">Therefore, we recommend that admins verify the free space in the archive mailbox, which allows the user to continue using the archive mailbox while it expands.</span></span> <span data-ttu-id="b8cef-115">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ภาพรวมของการเก็บถาวรแบบไม่จำกัดใน microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving)และ[เปิดใช้งานการเก็บถาวรแบบไม่จำกัดใน microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving)</span><span class="sxs-lookup"><span data-stu-id="b8cef-115">For more information, see [Overview of unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) and [Enable unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).</span></span>

<span data-ttu-id="b8cef-116">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเข้าถึงกล่องจดหมายเก็บถาวรจาก Outlook ให้ดู[ที่ความต้องการของ outlook สำหรับการเข้าถึงรายการในที่เก็บถาวรที่ขยายอัตโนมัติ](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)</span><span class="sxs-lookup"><span data-stu-id="b8cef-116">For more information on accessing the archive mailbox from Outlook, see [Outlook requirements for accessing items in an auto-expanded archive](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive).</span></span> <span data-ttu-id="b8cef-117">เมื่อต้องการกำหนดค่านโยบายการเก็บข้อมูลที่จะย้ายรายการไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติให้ดูที่[ตั้งค่านโยบายการเก็บถาวรและการลบสำหรับกล่องจดหมายในองค์กร Microsoft ๓๖๕ของคุณ](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="b8cef-117">To configure a retention policy that automatically moves items to the archive mailbox, see [Set up an archive and deletion policy for mailboxes in your Microsoft 365 organization](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).</span></span>

<span data-ttu-id="b8cef-118">**หมายเหตุ**: ที่เก็บถาวรที่ขยายอัตโนมัติไม่ได้รับการสนับสนุนสำหรับกล่องจดหมายหลักบน Exchange ๒๐๑๐</span><span class="sxs-lookup"><span data-stu-id="b8cef-118">**Note**: Auto-expanding archives aren't supported for primary mailboxes on Exchange 2010.</span></span>
