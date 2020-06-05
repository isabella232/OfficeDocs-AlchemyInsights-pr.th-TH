---
title: อีเมลที่ขาดไปในเขตกักกัน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569562"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="6354c-102">อีเมลที่ขาดหายไปในเขตกักกัน"</span><span class="sxs-lookup"><span data-stu-id="6354c-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="6354c-103">ผู้ดูแลระบบสามารถดู[ปล่อย หรือลบข้อความเหล่านี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="6354c-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="6354c-104">เมื่อต้องการเปิดศูนย์การปฏิบัติตามกฎระเบียบ&ความปลอดภัย ให้ไปที่ [https://protection.office.com](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="6354c-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="6354c-105">เมื่อต้องการเปิดหน้าการกักกันโดยตรง ให้ไปที่ [https://protection.office.com/quarantine](https://protection.office.com/quarantine)</span><span class="sxs-lookup"><span data-stu-id="6354c-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="6354c-106">คุณสามารถค้นหาตามค่าต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="6354c-106">You can search by the following values:</span></span>  

- <span data-ttu-id="6354c-107">**รหัสข้อความ**: ตัวระบุที่ไม่ซ้ํากันทั่วโลกของข้อความ</span><span class="sxs-lookup"><span data-stu-id="6354c-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="6354c-108">ถ้าคุณเลือกข้อความในรายการ ค่า**ID ข้อความ\*\*\*\*จะปรากฏขึ้นในบานหน้าต่างลอย**รายละเอียดที่ปรากฏขึ้น</span><span class="sxs-lookup"><span data-stu-id="6354c-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="6354c-109">ผู้ดูแลระบบสามารถใช้[การติดตามข้อความ](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide)เพื่อค้นหาข้อความและค่ารหัสข้อความที่สอดคล้องกันได้</span><span class="sxs-lookup"><span data-stu-id="6354c-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="6354c-110">**ที่อยู่อีเมลผู้ส่ง**: ที่อยู่อีเมลของผู้ส่งรายเดียว</span><span class="sxs-lookup"><span data-stu-id="6354c-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="6354c-111">**ที่อยู่อีเมลของผู้รับ**: ที่อยู่อีเมลของผู้รับรายเดียว</span><span class="sxs-lookup"><span data-stu-id="6354c-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="6354c-112">**เรื่อง**: ใช้เรื่องทั้งหมดของข้อความ</span><span class="sxs-lookup"><span data-stu-id="6354c-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="6354c-113">การค้นหาไม่ตรงตามตัวพิมพ์ใหญ่-เล็ก</span><span class="sxs-lookup"><span data-stu-id="6354c-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="6354c-114">หลังจากที่คุณป้อนเกณฑ์การค้นหาแล้ว ให้คลิกปุ่ม ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **รีเฟรช**เพื่อกรองผลลัพธ์  </span><span class="sxs-lookup"><span data-stu-id="6354c-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="6354c-115">cmdlets ที่คุณใช้เพื่อดูและจัดการข้อความและไฟล์ในกักกันได้แก่:</span><span class="sxs-lookup"><span data-stu-id="6354c-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="6354c-116">ลบ-กักกัน</span><span class="sxs-lookup"><span data-stu-id="6354c-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="6354c-117">ส่งออก-กักกัน</span><span class="sxs-lookup"><span data-stu-id="6354c-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="6354c-118">รับ-กักกัน</span><span class="sxs-lookup"><span data-stu-id="6354c-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="6354c-119">[การแสดงตัวอย่าง-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)โปรดทราบว่า cmdlet นี้สําหรับข้อความเท่านั้น ไม่ใช่แฟ้มมัลแวร์จาก ATP สําหรับ SharePoint Online, OneDrive สําหรับธุรกิจ หรือทีม</span><span class="sxs-lookup"><span data-stu-id="6354c-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="6354c-120">ปล่อย- กักกัน</span><span class="sxs-lookup"><span data-stu-id="6354c-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)