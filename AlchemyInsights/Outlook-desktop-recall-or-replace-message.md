---
title: การเรียกคืนบนเดสก์ท็อป outlook หรือแทนข้อความอีเมล
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657062"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="b04bc-102">การเรียกคืน หรือแทนข้อความอีเมล</span><span class="sxs-lookup"><span data-stu-id="b04bc-102">Recall or replace an email message</span></span>

- <span data-ttu-id="b04bc-103">เป็นผู้ดูแลระบบ คุณสามารถ**เรียกคืนข้อความในนามของผู้ใช้ที่ใช้ PowerShell**</span><span class="sxs-lookup"><span data-stu-id="b04bc-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="b04bc-104">คุณไม่สามารถเรียกคืนข้อความจากศูนย์ดูแล</span><span class="sxs-lookup"><span data-stu-id="b04bc-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="b04bc-105">คุณสามารถ**เฉพาะข้อความเรียกคืนซึ่งจะถูกส่งไปยังบุคคลในองค์กรของคุณ**</span><span class="sxs-lookup"><span data-stu-id="b04bc-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="b04bc-106">ถ้าข้อความถูกส่งไปยังที่อยู่ Gmail ตัวอย่างเช่น คุณไม่สามารถเรียกคืนนั้น</span><span class="sxs-lookup"><span data-stu-id="b04bc-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="b04bc-107">คุณสามารถ**เฉพาะข้อความเรียกคืนส่งจาก Outlook 2016 บนพีซีแบบ**</span><span class="sxs-lookup"><span data-stu-id="b04bc-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="b04bc-108">ถ้าผู้ใช้ส่งข้อความโดยใช้ Outlook สำหรับ Mac หรือ Outlook บนเว็บ คุณไม่สามารถเรียกคืน</span><span class="sxs-lookup"><span data-stu-id="b04bc-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="b04bc-109">เมื่อต้องการเรียกคืน หรือแทนข้อความอีเมล:</span><span class="sxs-lookup"><span data-stu-id="b04bc-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="b04bc-110">ในบานหน้าต่างโฟลเดอร์ทางด้านซ้ายของหน้าต่าง Outlook เลือกโฟลเดอร์รายการที่ถูกส่ง</span><span class="sxs-lookup"><span data-stu-id="b04bc-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="b04bc-111">คลิกสองครั้งที่ข้อความคุณต้องการเรียกคืนเพื่อเปิดแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="b04bc-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="b04bc-112">เลือกแท็บ**ข้อความ**และจากนั้น เลือก**การกระทำ** > **เรียกคืนข้อความนี้**</span><span class="sxs-lookup"><span data-stu-id="b04bc-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="b04bc-113">เลือก**ลบสำเนาที่ยังไม่ได้อ่านของข้อความนี้**หรือ**ลบสำเนาที่ยังไม่ได้อ่าน และแทนที่ ด้วยข้อความใหม่**และจากนั้น ให้เลือก **'ตกลง'**</span><span class="sxs-lookup"><span data-stu-id="b04bc-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="b04bc-114">ถ้าคุณกำลังส่งข้อความแทน เรียบเรียงข้อความ จากนั้น**ส่ง**</span><span class="sxs-lookup"><span data-stu-id="b04bc-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="b04bc-115">ความสำเร็จหรือความล้มเหลวของการเรียกคืนข้อความขึ้นอยู่กับการตั้งค่าของผู้รับใน Outlook</span><span class="sxs-lookup"><span data-stu-id="b04bc-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="b04bc-116">สำหรับขั้นตอนการตรวจสอบในการเรียกคืน ดู[บทความนี้](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)</span><span class="sxs-lookup"><span data-stu-id="b04bc-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="b04bc-117">ค้นหา และลบข้อความอีเมลในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="b04bc-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="b04bc-118">ถ้าคุณไม่ได้เป็นผู้ดูแลส่วนกลาง บัญชีของคุณต้องเพิ่มบทบาทผู้จัดการ eDiscovery หรือบทบาทการบริหารการปฏิบัติตามกฎระเบียบการค้นหาเพื่อค้นหาข้อความ</span><span class="sxs-lookup"><span data-stu-id="b04bc-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="b04bc-119">การลบข้อความ คุณจำเป็นต้องเข้าร่วมกลุ่มบทบาทการจัดการองค์กรหรือบทบาทจัดการค้นหาและกำจัด</span><span class="sxs-lookup"><span data-stu-id="b04bc-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="b04bc-120">สิทธิ์สำหรับบทบาทเหล่านี้จะถูกกำหนดใน[ศูนย์การรักษาความปลอดภัยและความสอดคล้อง](https://go.microsoft.com/fwlink/?linkid=2083731)กัน</span><span class="sxs-lookup"><span data-stu-id="b04bc-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="b04bc-121">การ[สร้างเนื้อหามีการค้นหา](https://docs.microsoft.com/office365/securitycompliance/content-search)เพื่อค้นหาข้อความที่จะลบ</span><span class="sxs-lookup"><span data-stu-id="b04bc-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="b04bc-122">[เชื่อมต่อกับ PowerShell ศูนย์ปฏิบัติตามกฎระเบียบและการรักษาความปลอดภัย](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="b04bc-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="b04bc-123">ถ้าคุณกำลังใช้การรับรองความถูกต้องด้วยหลายปัจจัย ดูการ[เชื่อมต่อกับ Office 365 ปลอดภัยและปฏิบัติตามกฎระเบียบศูนย์ PowerShell โดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="b04bc-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>