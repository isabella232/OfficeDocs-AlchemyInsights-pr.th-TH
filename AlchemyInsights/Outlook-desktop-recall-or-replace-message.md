---
title: การเรียกคืนหรือแทนที่ข้อความอีเมล
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687529"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="8a199-102">เรียกคืนหรือแทนที่ข้อความอีเมล Outlook</span><span class="sxs-lookup"><span data-stu-id="8a199-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="8a199-103">ในฐานะผู้ดูแลระบบ คุณสามารถ**เรียกคืนข้อความในนามของผู้ใช้โดยใช้ PowerShell**</span><span class="sxs-lookup"><span data-stu-id="8a199-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="8a199-104">คุณไม่สามารถเรียกคืนข้อความจากศูนย์การจัดการได้</span><span class="sxs-lookup"><span data-stu-id="8a199-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="8a199-105">คุณสามารถ**เรียกคืนข้อความที่ถูกส่งไปยังบุคคลในองค์กรของคุณเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="8a199-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="8a199-106">ตัวอย่างเช่น หากข้อความดังกล่าวส่งไปยังที่อยู่ Gmail คุณจะไม่สามารถเรียกคืนได้</span><span class="sxs-lookup"><span data-stu-id="8a199-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="8a199-107">คุณสามารถ**เรียกคืนข้อความที่ส่งจาก Outlook 2016 บนพีซีเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="8a199-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="8a199-108">ถ้าผู้ใช้ส่งข้อความโดยใช้ Outlook สําหรับ Mac หรือ Outlook บนเว็บ คุณจะไม่สามารถเรียกคืนได้</span><span class="sxs-lookup"><span data-stu-id="8a199-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="8a199-109">เมื่อต้องการเรียกคืนหรือแทนที่ข้อความอีเมล ให้ทําดังนี้</span><span class="sxs-lookup"><span data-stu-id="8a199-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="8a199-110">ในบานหน้าต่างโฟลเดอร์ทางด้านซ้ายของหน้าต่าง Outlook ให้เลือกโฟลเดอร์ รายการที่ถูกส่ง</span><span class="sxs-lookup"><span data-stu-id="8a199-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="8a199-111">คลิกสองครั้งที่ข้อความที่คุณต้องการเรียกคืนเพื่อเปิด</span><span class="sxs-lookup"><span data-stu-id="8a199-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="8a199-112">เลือกแท็บ**ข้อความ**แล้วเลือก**การกระทํา** > **เรียกคืนข้อความนี้**</span><span class="sxs-lookup"><span data-stu-id="8a199-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="8a199-113">เลือก**ลบสําเนาที่ยังไม่ได้อ่าน ของข้อความนี้**หรือ**ลบสําเนาที่ยังไม่ได้อ่าน แล้วแทนที่ด้วยข้อความใหม่**แล้วเลือก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="8a199-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="8a199-114">ถ้าคุณกําลังส่งข้อความแทนที่ ให้เขียนข้อความ แล้วเลือก**ส่ง**</span><span class="sxs-lookup"><span data-stu-id="8a199-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="8a199-115">ความสําเร็จหรือความล้มเหลวของการเรียกคืนข้อความขึ้นอยู่กับการตั้งค่าของผู้รับใน Outlook</span><span class="sxs-lookup"><span data-stu-id="8a199-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="8a199-116">สําหรับขั้นตอนในการตรวจสอบการเรียกคืน ให้ดูที่[บทความนี้](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)</span><span class="sxs-lookup"><span data-stu-id="8a199-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="8a199-117">ค้นหาและลบข้อความอีเมลในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="8a199-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="8a199-118">ถ้าคุณไม่ใช่ผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="8a199-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="8a199-119">เมื่อต้องการลบข้อความ คุณจะต้องเข้าร่วมกลุ่มบทบาทการจัดการองค์กร หรือบทบาทการจัดการการค้นหาและการล้างข้อมูล</span><span class="sxs-lookup"><span data-stu-id="8a199-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="8a199-120">สิทธิการได้รับอนุญาตสําหรับบทบาทเหล่านี้จะถูกกําหนดใน[ศูนย์ความปลอดภัยและการปฏิบัติตามกฎระเบียบ](https://go.microsoft.com/fwlink/?linkid=2083731)</span><span class="sxs-lookup"><span data-stu-id="8a199-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="8a199-121">[สร้างการค้นหาเนื้อหา](https://docs.microsoft.com/office365/securitycompliance/content-search)เพื่อค้นหาข้อความที่จะลบ</span><span class="sxs-lookup"><span data-stu-id="8a199-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="8a199-122">[เชื่อมต่อกับศูนย์ความปลอดภัยและการปฏิบัติตามกฎระเบียบ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="8a199-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="8a199-123">ถ้าคุณกําลังใช้การรับรองความถูกต้องด้วยหลายปัจจัย ให้ดูที่[เชื่อมต่อกับการรักษาความปลอดภัย Microsoft 365 และ PowerShell ศูนย์การปฏิบัติตามกฎระเบียบโดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="8a199-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>