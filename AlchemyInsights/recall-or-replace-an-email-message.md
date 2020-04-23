---
title: การเรียกคืนหรือแทนที่ข้อความอีเมล
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e541620a499b02a7206579ffcc505ceb4e632a4c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742774"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="d8c51-102">เรียกคืนหรือแทนที่ข้อความอีเมลใน Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d8c51-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="d8c51-103">คุณสามารถ**เรียกคืนข้อความที่ถูกส่งไปยังบุคคลในองค์กรของคุณเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="d8c51-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="d8c51-104">ตัวอย่างเช่น หากข้อความดังกล่าวส่งไปยังที่อยู่ Gmail คุณจะไม่สามารถเรียกคืนได้</span><span class="sxs-lookup"><span data-stu-id="d8c51-104">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="d8c51-105">คุณสามารถ**เรียกคืนข้อความที่ส่งจาก Outlook 2016 สําหรับพีซี**เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="d8c51-105">You can **only recall messages sent from Outlook 2016 for the PC**.</span></span> <span data-ttu-id="d8c51-106">ถ้าผู้ใช้ส่งข้อความโดยใช้ Outlook สําหรับ Mac หรือ Outlook บนเว็บ คุณจะไม่สามารถเรียกคืนได้</span><span class="sxs-lookup"><span data-stu-id="d8c51-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="d8c51-107">ถ้าคุณเป็นผู้ดูแลระบบ คุณสามารถ**เรียกคืนข้อความในนามของผู้ใช้โดยใช้ PowerShell**</span><span class="sxs-lookup"><span data-stu-id="d8c51-107">If you're an admin, you can **recall messages on behalf of users by using PowerShell**.</span></span> <span data-ttu-id="d8c51-108">คุณไม่สามารถเรียกคืนข้อความจากศูนย์การจัดการได้</span><span class="sxs-lookup"><span data-stu-id="d8c51-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="d8c51-109">เลื่อนลงไปที่ "ค้นหาและลบข้อความอีเมลในองค์กรของคุณ" เพื่อดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="d8c51-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="d8c51-110">**เรียกคืนหรือแทนที่ข้อความอีเมลที่คุณส่ง**</span><span class="sxs-lookup"><span data-stu-id="d8c51-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="d8c51-111">ในบานหน้าต่างโฟลเดอร์ทางด้านซ้ายของหน้าต่าง Outlook ให้เลือกโฟลเดอร์ รายการที่ถูกส่ง</span><span class="sxs-lookup"><span data-stu-id="d8c51-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="d8c51-112">เปิดข้อความที่คุณต้องการเรียกคืน</span><span class="sxs-lookup"><span data-stu-id="d8c51-112">Open the message that you want to recall.</span></span> <span data-ttu-id="d8c51-113">คุณต้องคลิกสองครั้งเพื่อเปิดข้อความ</span><span class="sxs-lookup"><span data-stu-id="d8c51-113">You must double-click to open the message.</span></span> <span data-ttu-id="d8c51-114">การเลือกข้อความเพื่อให้ข้อความปรากฏในบานหน้าต่างการอ่านจะไม่อนุญาตให้คุณเรียกคืนข้อความ</span><span class="sxs-lookup"><span data-stu-id="d8c51-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="d8c51-115">จากแท็บ ข้อความ ให้เลือก**การกระทํา** > **เรียกคืนข้อความนี้**</span><span class="sxs-lookup"><span data-stu-id="d8c51-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="d8c51-116">เลือก**ลบสําเนาที่ยังไม่ได้อ่านของข้อความนี้**หรือ**ลบสําเนาที่ยังไม่ได้อ่าน แล้วแทนที่ด้วยข้อความใหม่**จากนั้นเลือก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="d8c51-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="d8c51-117">ถ้าคุณกําลังส่งข้อความที่เปลี่ยนให้เขียนข้อความ จากนั้นเลือก**ส่ง**</span><span class="sxs-lookup"><span data-stu-id="d8c51-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="d8c51-118">ความสําเร็จหรือความล้มเหลวของการเรียกคืนข้อความขึ้นอยู่กับการตั้งค่าของผู้รับใน Outlook</span><span class="sxs-lookup"><span data-stu-id="d8c51-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="d8c51-119">สําหรับข้อมูลเพิ่มเติม รวมทั้งวิธีการตรวจสอบในการเรียกคืน ให้ดูที่[การเรียกคืนหรือแทนที่ข้อความอีเมลที่คุณส่ง](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)</span><span class="sxs-lookup"><span data-stu-id="d8c51-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="d8c51-120">***ค้นหาและลบข้อความอีเมลในองค์กรของคุณ*** เมื่อต้องการค้นหาและลบข้อความอีเมลในองค์กรของคุณ จะเป็นการง่ายที่สุดถ้าคุณเป็นผู้ดูแลระบบส่วนกลาง ถ้าคุณไม่ใช่ผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="d8c51-120">***Search for and delete email messages in your organization*** To search for and delete email messages in your organization, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="d8c51-121">เมื่อต้องการลบข้อความ คุณจะต้องเข้าร่วมกลุ่มบทบาทการจัดการองค์กร หรือบทบาทการจัดการการค้นหาและการล้างข้อมูล</span><span class="sxs-lookup"><span data-stu-id="d8c51-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="d8c51-122">สิทธิการได้รับอนุญาตสําหรับบทบาทเหล่านี้จะถูกกําหนดใน[ศูนย์การปฏิบัติตามกฎระเบียบความปลอดภัย &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="d8c51-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="d8c51-123">[สร้างการค้นหาเนื้อหา](https://docs.microsoft.com/office365/securitycompliance/content-search)เพื่อค้นหาข้อความที่จะลบ</span><span class="sxs-lookup"><span data-stu-id="d8c51-123">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="d8c51-124">[เชื่อมต่อกับศูนย์การปฏิบัติตามกฎระเบียบ&ความปลอดภัย PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="d8c51-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span> 

<span data-ttu-id="d8c51-125">ถ้าคุณกําลังใช้ MFA โปรดดูที่[เชื่อมต่อกับการรักษาความปลอดภัย Microsoft 365 & PowerShell ศูนย์การปฏิบัติตามกฎระเบียบโดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="d8c51-125">If you're using MFA, see [Connect to Microsoft 365 security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span> 
