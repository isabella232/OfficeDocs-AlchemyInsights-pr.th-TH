---
title: การเรียกคืนหรือแทนที่ข้อความอีเมล
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353525"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="35744-102">การเรียกคืนหรือแทนที่ข้อความอีเมลใน Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="35744-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="35744-103">คุณสามารถ **เรียกคืนข้อความที่ถูกส่งไปยังบุคคลในองค์กรของคุณเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="35744-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="35744-104">ตัวอย่างเช่นถ้าข้อความถูกส่งไปยังที่อยู่ Gmail คุณจะไม่สามารถเรียกคืนได้</span><span class="sxs-lookup"><span data-stu-id="35744-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="35744-105">คุณสามารถ **เรียกคืนได้เฉพาะข้อความที่ส่งจาก Outlook สำหรับพีซีเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="35744-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="35744-106">ถ้าผู้ใช้ส่งข้อความโดยใช้ Outlook for Mac หรือ Outlook บนเว็บคุณจะไม่สามารถเรียกคืนได้</span><span class="sxs-lookup"><span data-stu-id="35744-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="35744-107">ในฐานะผู้ดูแลผู้เช่าคุณสามารถ **เรียกคืนข้อความในนามของผู้ใช้โดยใช้ PowerShell** (สำหรับข้อมูลเพิ่มเติมให้ดูที่ [ค้นหาและลบข้อความอีเมล](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization))</span><span class="sxs-lookup"><span data-stu-id="35744-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="35744-108">คุณไม่สามารถเรียกคืนข้อความจากศูนย์การจัดการได้</span><span class="sxs-lookup"><span data-stu-id="35744-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="35744-109">เลื่อนลงไปที่ "ค้นหาและลบข้อความอีเมลในองค์กรของคุณ" สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="35744-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="35744-110">**การเรียกคืนหรือแทนที่ข้อความอีเมลที่คุณส่ง**</span><span class="sxs-lookup"><span data-stu-id="35744-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="35744-111">ในบานหน้าต่างโฟลเดอร์ทางด้านซ้ายของหน้าต่าง Outlook ให้เลือกโฟลเดอร์รายการที่ถูกส่ง</span><span class="sxs-lookup"><span data-stu-id="35744-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="35744-112">เปิดข้อความที่คุณต้องการเรียกคืน</span><span class="sxs-lookup"><span data-stu-id="35744-112">Open the message that you want to recall.</span></span> <span data-ttu-id="35744-113">คุณต้องดับเบิลคลิกเพื่อเปิดข้อความ</span><span class="sxs-lookup"><span data-stu-id="35744-113">You must double-click to open the message.</span></span> <span data-ttu-id="35744-114">การเลือกข้อความเพื่อให้ปรากฏในบานหน้าต่างการอ่านจะไม่อนุญาตให้คุณเรียกคืนข้อความได้</span><span class="sxs-lookup"><span data-stu-id="35744-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="35744-115">จากแท็บข้อความให้เลือก **การดำเนินการ**  >  **เรียกคืนข้อความนี้**</span><span class="sxs-lookup"><span data-stu-id="35744-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="35744-116">เลือก **ลบสำเนาที่ยังไม่ได้อ่านของข้อความนี้** หรือ **ลบสำเนาที่ยังไม่ได้อ่านและแทนที่ด้วยข้อความใหม่** จากนั้นเลือก **ตกลง**</span><span class="sxs-lookup"><span data-stu-id="35744-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="35744-117">ถ้าคุณกำลังส่งข้อความทดแทนให้เขียนข้อความจากนั้นเลือก **ส่ง**</span><span class="sxs-lookup"><span data-stu-id="35744-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="35744-118">ความสำเร็จหรือความล้มเหลวของการเรียกคืนข้อความจะขึ้นอยู่กับการตั้งค่าของผู้รับใน Outlook</span><span class="sxs-lookup"><span data-stu-id="35744-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="35744-119">สำหรับข้อมูลเพิ่มเติมรวมถึงวิธีการตรวจสอบการเรียกคืนให้ดู[ที่เรียกคืนหรือแทนที่ข้อความอีเมลที่คุณส่ง](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)</span><span class="sxs-lookup"><span data-stu-id="35744-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="35744-120">**_เมื่อต้องการค้นหาและลบข้อความอีเมลในองค์กรของคุณ_** คุณจะสามารถทำงานได้ง่ายที่สุดถ้าคุณเป็นผู้ดูแลส่วนกลาง ถ้าคุณไม่ใช่ผู้ดูแลระบบส่วนกลางบัญชีผู้ใช้ของคุณจะต้องถูกเพิ่มลงในกลุ่มบทบาทผู้จัดการ eDiscovery หรือไปยังบทบาทการจัดการการค้นหาการปฏิบัติตามกฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="35744-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="35744-121">เมื่อต้องการลบข้อความคุณจะต้องเข้าร่วมกลุ่มบทบาทการจัดการองค์กรหรือบทบาทการจัดการการค้นหาและการล้างข้อมูล</span><span class="sxs-lookup"><span data-stu-id="35744-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="35744-122">สิทธิ์ของบทบาทเหล่านี้จะได้รับการกำหนดใน[ศูนย์การปฏิบัติตามกฎระเบียบ & ด้านความปลอดภัย](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="35744-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="35744-123">[สร้างการค้นหาเนื้อหา](https://docs.microsoft.com/microsoft-365/compliance/content-search) เพื่อค้นหาข้อความที่จะลบ</span><span class="sxs-lookup"><span data-stu-id="35744-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="35744-124">[เชื่อมต่อกับการรักษาความปลอดภัย & ศูนย์การปฏิบัติตามนโยบายของ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="35744-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="35744-125">ถ้าคุณกำลังใช้ MFA (การรับรองความถูกต้องแบบหลายปัจจัย) ให้ดู[ที่เชื่อมต่อกับ Microsoft ๓๖๕ & Security ศูนย์การปฏิบัติตามนโยบายของ Microsoft โดยใช้การรับรองความถูกต้องแบบหลายปัจจัย](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="35744-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
