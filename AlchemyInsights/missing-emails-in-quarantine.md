---
title: อีเมลหายไปในการกักกัน
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539843"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="c3e18-102">อีเมลหายไปในการกักกัน"</span><span class="sxs-lookup"><span data-stu-id="c3e18-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="c3e18-103">ผู้ดูแลระบบสามารถดู [เผยแพร่ หรือลบข้อความเหล่านี้ได้](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="c3e18-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="c3e18-104">เมื่อต้องการเปิดศูนย์&การปฏิบัติตามนโยบาย [https://protection.office.com](https://protection.office.com/) ให้ไปที่</span><span class="sxs-lookup"><span data-stu-id="c3e18-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="c3e18-105">เมื่อต้องการเปิดหน้า การกักกัน โดยตรง ให้ไปที่ [https://protection.office.com/quarantine](https://protection.office.com/quarantine)</span><span class="sxs-lookup"><span data-stu-id="c3e18-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="c3e18-106">คุณสามารถค้นหาด้วยค่าต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="c3e18-106">You can search by the following values:</span></span>  

- <span data-ttu-id="c3e18-107">**ID ข้อความ**: ตัวระบุที่ไม่รหัสเฉพาะส่วนกลางของข้อความ</span><span class="sxs-lookup"><span data-stu-id="c3e18-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="c3e18-108">ถ้าคุณเลือกข้อความในรายการ ค่า  **ID**  ข้อความจะปรากฏขึ้นในบานหน้าต่าง  **แถบปลิว**  รายละเอียด ที่ปรากฏขึ้น</span><span class="sxs-lookup"><span data-stu-id="c3e18-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="c3e18-109">ผู้ดูแลระบบสามารถใช้การติดตาม [ข้อความเพื่อค้นหา](/microsoft-365/security/office-365-security/message-trace-scc) ข้อความและค่า ID ข้อความที่สอดคล้องกัน</span><span class="sxs-lookup"><span data-stu-id="c3e18-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="c3e18-110">**ที่อยู่อีเมลผู้ส่ง**: ที่อยู่อีเมลของผู้ส่งเดียว</span><span class="sxs-lookup"><span data-stu-id="c3e18-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="c3e18-111">**ที่อยู่อีเมลผู้รับ**: ที่อยู่อีเมลของผู้รับเดียว</span><span class="sxs-lookup"><span data-stu-id="c3e18-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="c3e18-112">**เรื่อง**: ใช้ชื่อเรื่องทั้งหมดของข้อความ</span><span class="sxs-lookup"><span data-stu-id="c3e18-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="c3e18-113">การค้นหาไม่ตรงตามตัวพิมพ์ใหญ่-เล็ก</span><span class="sxs-lookup"><span data-stu-id="c3e18-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="c3e18-114">หลังจากที่คุณใส่เกณฑ์การค้นหา ให้คลิกปุ่ม รีเฟรช ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **รีเฟรช** เพื่อกรองผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="c3e18-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="c3e18-115">cmdlet ที่คุณใช้เพื่อดูและจัดการข้อความและไฟล์ในการกักกันคือ:</span><span class="sxs-lookup"><span data-stu-id="c3e18-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="c3e18-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="c3e18-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="c3e18-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="c3e18-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="c3e18-118">Get-quarantineMessage</span><span class="sxs-lookup"><span data-stu-id="c3e18-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="c3e18-119">[การกักกันแสดงตัวอย่าง :](/powershell/module/exchange/preview-quarantinemessage)โปรดทราบว่า cmdlet นี้จะมีไว้เฉพาะข้อความเท่านั้น ไม่ใช่ไฟล์มัลแวร์จาก Microsoft Defender Office 365 for SharePoint Online, OneDrive for Business หรือ Teams</span><span class="sxs-lookup"><span data-stu-id="c3e18-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="c3e18-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="c3e18-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)