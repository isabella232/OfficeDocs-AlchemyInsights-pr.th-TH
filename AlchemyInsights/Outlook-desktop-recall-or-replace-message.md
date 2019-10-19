---
title: การเรียกคืนเดสก์ท็อปของ Outlook หรือแทนที่ข้อความทางเมล
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36496130"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="ecc2f-102">เรียกคืนหรือแทนที่ข้อความ email Outlook</span><span class="sxs-lookup"><span data-stu-id="ecc2f-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="ecc2f-103">ในฐานะที่เป็นผู้ดูแลระบบคุณสามารถ**เรียกคืนข้อความในนามของผู้ใช้ที่ใช้ PowerShell**</span><span class="sxs-lookup"><span data-stu-id="ecc2f-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="ecc2f-104">คุณไม่สามารถเรียกคืนข้อความจากศูนย์การจัดการได้</span><span class="sxs-lookup"><span data-stu-id="ecc2f-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="ecc2f-105">คุณสามารถ**เรียกคืนข้อความที่ส่งถึงผู้คนในองค์กรของคุณเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="ecc2f-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="ecc2f-106">ตัวอย่างเช่นหากส่งข้อความไปยังที่อยู่ Gmail คุณจะไม่สามารถเรียกคืนได้</span><span class="sxs-lookup"><span data-stu-id="ecc2f-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="ecc2f-107">คุณสามารถ**เรียกคืนข้อความที่ส่งจาก Outlook ๒๐๑๖บนพีซีเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="ecc2f-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="ecc2f-108">ถ้าผู้ใช้ส่งข้อความโดยใช้ Outlook สำหรับ Mac หรือ Outlook บนเว็บคุณจะไม่สามารถเรียกคืนได้</span><span class="sxs-lookup"><span data-stu-id="ecc2f-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="ecc2f-109">วิธีการเรียกคืนหรือแทนที่ข้อความในเมล:</span><span class="sxs-lookup"><span data-stu-id="ecc2f-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="ecc2f-110">ในบานหน้าต่างโฟลเดอร์ที่ด้านซ้ายของหน้าต่าง Outlook ให้เลือกโฟลเดอร์รายการที่ถูกส่ง</span><span class="sxs-lookup"><span data-stu-id="ecc2f-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="ecc2f-111">คลิกสองครั้งที่ข้อความที่คุณต้องการเรียกคืนเพื่อเปิด</span><span class="sxs-lookup"><span data-stu-id="ecc2f-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="ecc2f-112">เลือกแท็บ**ข้อความ**จากนั้นเลือก**การดำเนินการ** > **เรียกคืนข้อความนี้**</span><span class="sxs-lookup"><span data-stu-id="ecc2f-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="ecc2f-113">เลือก**ลบสำเนาที่ยังไม่ได้อ่านของข้อความนี้**หรือ**ลบสำเนาที่ยังไม่ได้อ่านและแทนที่ด้วยข้อความใหม่**และจากนั้นให้เลือก **' ตกลง '**</span><span class="sxs-lookup"><span data-stu-id="ecc2f-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="ecc2f-114">หากคุณกำลังส่งข้อความแทนที่ให้เขียนข้อความแล้วเลือก**ส่ง**</span><span class="sxs-lookup"><span data-stu-id="ecc2f-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="ecc2f-115">ความสำเร็จหรือล้มเหลวของการเรียกคืนข้อความขึ้นอยู่กับการตั้งค่าของผู้รับใน Outlook</span><span class="sxs-lookup"><span data-stu-id="ecc2f-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="ecc2f-116">สำหรับขั้นตอนในการตรวจสอบการเรียกคืนโปรดดู[บทความนี้](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)</span><span class="sxs-lookup"><span data-stu-id="ecc2f-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="ecc2f-117">ค้นหาและลบข้อความทางเมลในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="ecc2f-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="ecc2f-118">ถ้าคุณไม่ใช่ผู้ดูแลส่วนกลางบัญชีของคุณจะต้องถูกเพิ่มลงในบทบาทผู้จัดการ eDiscovery หรือบทบาทการจัดการการค้นหาการปฏิบัติตามกฎระเบียบเพื่อค้นหาข้อความ</span><span class="sxs-lookup"><span data-stu-id="ecc2f-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="ecc2f-119">ในการลบข้อความคุณจะต้องเข้าร่วมกลุ่มบทบาทการจัดการองค์กรหรือบทบาทการจัดการการค้นหาและล้างข้อมูล</span><span class="sxs-lookup"><span data-stu-id="ecc2f-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="ecc2f-120">สิทธิ์สำหรับบทบาทเหล่านี้จะถูกกำหนดใน[ศูนย์ความปลอดภัยและการปฏิบัติตามกฎระเบียบ](https://go.microsoft.com/fwlink/?linkid=2083731)</span><span class="sxs-lookup"><span data-stu-id="ecc2f-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="ecc2f-121">[สร้างการค้นหาเนื้อหา](https://docs.microsoft.com/office365/securitycompliance/content-search)เพื่อค้นหาข้อความที่จะลบ</span><span class="sxs-lookup"><span data-stu-id="ecc2f-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="ecc2f-122">[เชื่อมต่อกับ PowerShell ศูนย์การรักษาความปลอดภัยและการปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="ecc2f-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="ecc2f-123">ถ้าคุณกำลังใช้การรับรองความถูกต้องด้วยหลายปัจจัยโปรดดู[ที่การเชื่อมต่อกับ Office ๓๖๕ศูนย์ความปลอดภัยและการปฏิบัติตามกฎระเบียบ PowerShell โดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="ecc2f-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>