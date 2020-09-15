---
title: อีเมลที่ขาดหายไปในการตรวจสอบสินค้า
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673733"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="1d773-102">อีเมลที่ขาดหายไปในกักกัน "</span><span class="sxs-lookup"><span data-stu-id="1d773-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="1d773-103">ผู้ดูแลระบบสามารถ [ดูวางจำหน่ายหรือลบข้อความเหล่านี้ได้](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="1d773-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="1d773-104">เมื่อต้องการเปิดศูนย์การปฏิบัติตามนโยบาย & ด้านความปลอดภัยให้ [https://protection.office.com](https://protection.office.com/) ไปที่</span><span class="sxs-lookup"><span data-stu-id="1d773-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="1d773-105">เมื่อต้องการเปิดหน้าการตรวจสอบสินค้าโดยตรงให้ [https://protection.office.com/quarantine](https://protection.office.com/quarantine) ไปที่</span><span class="sxs-lookup"><span data-stu-id="1d773-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="1d773-106">คุณสามารถค้นหาโดยใช้ค่าต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="1d773-106">You can search by the following values:</span></span>  

- <span data-ttu-id="1d773-107">**รหัสข้อความ**: ตัวระบุที่ไม่ซ้ำกันทั่วโลกของข้อความ</span><span class="sxs-lookup"><span data-stu-id="1d773-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="1d773-108">ถ้าคุณเลือกข้อความในรายการค่า  **ID ข้อความ**  จะปรากฏขึ้นในบานหน้าต่างเมนูลอย  **รายละเอียด**  ที่ปรากฏขึ้น</span><span class="sxs-lookup"><span data-stu-id="1d773-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="1d773-109">ผู้ดูแลระบบสามารถใช้การ [ติดตามข้อความ](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) เพื่อค้นหาข้อความและค่า ID ข้อความที่สอดคล้องกันได้</span><span class="sxs-lookup"><span data-stu-id="1d773-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="1d773-110">**ที่อยู่อีเมลของผู้ส่ง**: ที่อยู่อีเมลของผู้ส่งรายเดียว</span><span class="sxs-lookup"><span data-stu-id="1d773-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="1d773-111">**ที่อยู่อีเมลของผู้รับ**: ที่อยู่อีเมลของผู้รับรายเดียว</span><span class="sxs-lookup"><span data-stu-id="1d773-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="1d773-112">**เรื่อง**: ใช้ทั้งชื่อเรื่องของข้อความ</span><span class="sxs-lookup"><span data-stu-id="1d773-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="1d773-113">การค้นหาไม่ตรงตามตัวพิมพ์ใหญ่-เล็ก</span><span class="sxs-lookup"><span data-stu-id="1d773-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="1d773-114">หลังจากที่คุณใส่เกณฑ์การค้นหาแล้วให้คลิกรีเฟรช ![ ปุ่มรี ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **เฟรช**เพื่อกรองผลลัพธ์  </span><span class="sxs-lookup"><span data-stu-id="1d773-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="1d773-115">Cmdlets ที่คุณใช้ในการดูและจัดการข้อความและไฟล์ในการกักกันได้แก่</span><span class="sxs-lookup"><span data-stu-id="1d773-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="1d773-116">ลบ-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1d773-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="1d773-117">ส่งออก-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1d773-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="1d773-118">รับ-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1d773-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="1d773-119">[ตัวอย่าง-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): โปรดสังเกตว่า cmdlet นี้มีไว้สำหรับข้อความเท่านั้นไม่ใช่ไฟล์มัลแวร์จาก ATP สำหรับ SharePoint Online, OneDrive for Business หรือทีม</span><span class="sxs-lookup"><span data-stu-id="1d773-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="1d773-120">การวางจำหน่าย-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1d773-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)