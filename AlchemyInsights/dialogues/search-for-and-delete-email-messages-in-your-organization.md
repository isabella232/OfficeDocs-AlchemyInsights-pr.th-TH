---
title: ค้นหาและลบข้อความอีเมลในองค์กรของคุณ
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525444"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="36b89-102">ค้นหาและลบข้อความอีเมลในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="36b89-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="36b89-103">ให้ปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="36b89-103">Follow these steps:</span></span>

1. <span data-ttu-id="36b89-104">ถ้าคุณไม่ได้เป็นผู้ดูแลระบบส่วนกลาง เมื่อต้องการค้นหาข้อความที่บัญชีผู้ใช้ของคุณต้องเพิ่มลงในกลุ่มบทบาท **ตัวจัดการ eDiscovery** หรือ **บทบาทการจัดการการค้นหาการปฏิบัติตาม** นโยบาย</span><span class="sxs-lookup"><span data-stu-id="36b89-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="36b89-105">เมื่อต้องการลบข้อความ คุณจะต้องเข้าร่วมกลุ่มบทบาท **การจัดการองค์กร** หรือบทบาท **การจัดการการค้นหาและล้าง**</span><span class="sxs-lookup"><span data-stu-id="36b89-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="36b89-106">สิทธิ์ในบทบาทเหล่านี้ได้รับการมอบหมายใน [ศูนย์&การปฏิบัติตามนโยบาย](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="36b89-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="36b89-107">[สร้างการค้นหา](https://docs.microsoft.com/office365/securitycompliance/content-search) เนื้อหาเพื่อค้นหาข้อความเพื่อลบ</span><span class="sxs-lookup"><span data-stu-id="36b89-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="36b89-108">[เชื่อมต่อกับศูนย์&การปฏิบัติตามนโยบายของ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="36b89-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="36b89-109">ถ้าคุณใช้งาน MFA ให้ดูคําแนะนําเหล่านี้: เชื่อมต่อกับศูนย์การปฏิบัติตาม [& PowerShell โดยใช้การรับรองความถูกต้องโดยใช้หลายปัจจัย](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="36b89-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="36b89-110">ลบข้อความ: เรียกใช้ `New-ComplianceSearchAction` cmdlet เพื่อลบข้อความ</span><span class="sxs-lookup"><span data-stu-id="36b89-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="36b89-111">ข้อความที่ถูกลบจะถูกย้ายไปยังโฟลเดอร์รายการที่กู้คืนได้ของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="36b89-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="36b89-112">ตัวอย่างเช่น ดูขั้นตอนที่ [3: ลบข้อความ](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="36b89-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
