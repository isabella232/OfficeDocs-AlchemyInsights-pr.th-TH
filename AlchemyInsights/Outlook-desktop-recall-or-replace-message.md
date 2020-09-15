---
title: การเรียกคืนหรือแทนที่ข้อความอีเมลของ Outlook บนเดสก์ท็อป
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664009"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="1101f-102">การเรียกคืนหรือแทนที่ข้อความอีเมล Outlook</span><span class="sxs-lookup"><span data-stu-id="1101f-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="1101f-103">ในฐานะผู้ดูแลระบบคุณสามารถ **เรียกคืนข้อความในนามของผู้ใช้ที่ใช้ PowerShell**ได้</span><span class="sxs-lookup"><span data-stu-id="1101f-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="1101f-104">คุณไม่สามารถเรียกคืนข้อความจากศูนย์การจัดการได้</span><span class="sxs-lookup"><span data-stu-id="1101f-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="1101f-105">คุณสามารถ**เรียกคืนข้อความที่ถูกส่งไปยังบุคคลในองค์กรของคุณเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="1101f-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="1101f-106">ถ้าข้อความถูกส่งไปยังที่อยู่ Gmail ตัวอย่างเช่นคุณไม่สามารถเรียกคืนได้</span><span class="sxs-lookup"><span data-stu-id="1101f-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="1101f-107">คุณสามารถ**เรียกคืนได้เฉพาะข้อความที่ส่งจาก Outlook ๒๐๑๖บนพีซีเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="1101f-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="1101f-108">ถ้าผู้ใช้ส่งข้อความโดยใช้ Outlook for Mac หรือ Outlook บนเว็บคุณจะไม่สามารถเรียกคืนได้</span><span class="sxs-lookup"><span data-stu-id="1101f-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="1101f-109">เมื่อต้องการเรียกคืนหรือแทนที่ข้อความอีเมล:</span><span class="sxs-lookup"><span data-stu-id="1101f-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="1101f-110">ในบานหน้าต่างโฟลเดอร์ทางด้านซ้ายของหน้าต่าง Outlook ให้เลือกโฟลเดอร์รายการที่ถูกส่ง</span><span class="sxs-lookup"><span data-stu-id="1101f-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="1101f-111">ดับเบิลคลิกที่ข้อความที่คุณต้องการเรียกคืนเพื่อเปิดข้อความนั้น</span><span class="sxs-lookup"><span data-stu-id="1101f-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="1101f-112">เลือกแท็บ**ข้อความ**แล้วเลือก**การดำเนินการ**  >  **เรียกคืนข้อความนี้**</span><span class="sxs-lookup"><span data-stu-id="1101f-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="1101f-113">เลือก**ลบสำเนาที่ยังไม่ได้อ่านของข้อความนี้**หรือ**ลบสำเนาที่ยังไม่ได้อ่านและแทนที่ด้วยข้อความใหม่**แล้วเลือก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="1101f-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="1101f-114">ถ้าคุณกำลังส่งข้อความทดแทนให้เขียนข้อความแล้วเลือก**ส่ง**</span><span class="sxs-lookup"><span data-stu-id="1101f-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="1101f-115">ความสำเร็จหรือความล้มเหลวของการเรียกคืนข้อความจะขึ้นอยู่กับการตั้งค่าของผู้รับใน Outlook</span><span class="sxs-lookup"><span data-stu-id="1101f-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="1101f-116">สำหรับขั้นตอนในการตรวจสอบการเรียกคืนให้ดู[บทความนี้](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)</span><span class="sxs-lookup"><span data-stu-id="1101f-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="1101f-117">ค้นหาและลบข้อความอีเมลในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="1101f-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="1101f-118">ถ้าคุณไม่ใช่ผู้ดูแลระบบส่วนกลางบัญชีผู้ใช้ของคุณจะต้องถูกเพิ่มลงในบทบาทผู้จัดการ eDiscovery หรือบทบาทการจัดการการค้นหาการปฏิบัติตามกฎระเบียบเพื่อค้นหาข้อความ</span><span class="sxs-lookup"><span data-stu-id="1101f-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="1101f-119">เมื่อต้องการลบข้อความคุณจะต้องเข้าร่วมกลุ่มบทบาทการจัดการองค์กรหรือบทบาทการจัดการการค้นหาและการล้างข้อมูล</span><span class="sxs-lookup"><span data-stu-id="1101f-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="1101f-120">สิทธิ์สำหรับบทบาทเหล่านี้จะได้รับการกำหนดใน[ศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย](https://go.microsoft.com/fwlink/?linkid=2083731)</span><span class="sxs-lookup"><span data-stu-id="1101f-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="1101f-121">[สร้างการค้นหาเนื้อหา](https://docs.microsoft.com/microsoft-365/compliance/content-search) เพื่อค้นหาข้อความที่จะลบ</span><span class="sxs-lookup"><span data-stu-id="1101f-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="1101f-122">[เชื่อมต่อกับการรักษาความปลอดภัยและการปฏิบัติตามนโยบายศูนย์ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="1101f-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="1101f-123">ถ้าคุณกำลังใช้การรับรองความถูกต้องแบบหลายปัจจัยให้ดู[ที่เชื่อมต่อกับ Microsoft ๓๖๕ Security Center และการปฏิบัติตามนโยบายศูนย์การรับรองความถูกต้องโดยใช้การรับรองความถูกต้องแบบหลายปัจจัย](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="1101f-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>