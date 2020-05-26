---
title: นโยบายการแชร์ปฏิทิน 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373018"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="b34f4-102">ข้อผิดพลาดนโยบายเมื่อแชร์ปฏิทิน</span><span class="sxs-lookup"><span data-stu-id="b34f4-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="b34f4-103">ทําอย่างใดอย่างหนึ่งต่อไปนี้ ตามความเหมาะสมกับสถานการณ์ของคุณ:</span><span class="sxs-lookup"><span data-stu-id="b34f4-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="b34f4-104">เชื่อมต่อกับอัตราแลกเปลี่ยนแบบออนไลน์ โดยใช้ PowerShell ระยะไกล</span><span class="sxs-lookup"><span data-stu-id="b34f4-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="b34f4-105">สําหรับข้อมูลเพิ่มเติม ให้ดู[การเชื่อมต่อกับการแลกเปลี่ยนแบบออนไลน์โดยใช้ PowerShell ระยะไกล](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b34f4-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="b34f4-106">บนเซิร์ฟเวอร์ในสถานที่เปิดเชลล์จัดการการแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="b34f4-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="b34f4-107">กําหนดนโยบายการใช้ร่วมกันที่กําหนดให้กับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="b34f4-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="b34f4-108">เรียกใช้คําสั่งต่อไปนี้ และหมายเหตุนโยบายที่ส่งคืน:</span><span class="sxs-lookup"><span data-stu-id="b34f4-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="b34f4-109">ปรับปรุงนโยบายการใช้ร่วมกันสําหรับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="b34f4-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="b34f4-110">เมื่อต้องการทําเช่นนี้ ให้ทําตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="b34f4-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="b34f4-111">เปิดศูนย์การจัดการ Exchange</span><span class="sxs-lookup"><span data-stu-id="b34f4-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="b34f4-112">คลิก**องค์กร**แล้วคลิกสองครั้งที่นโยบายที่กําหนดให้กับผู้ใช้ภายใต้**การแชร์แต่ละบุคคล**</span><span class="sxs-lookup"><span data-stu-id="b34f4-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="b34f4-113">นี่คือนโยบายที่ถูกส่งกลับในขั้นตอนที่ 2</span><span class="sxs-lookup"><span data-stu-id="b34f4-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="b34f4-114">บนหน้า กฎการแชร์ ให้เลือกระดับการแชร์ปฏิทินที่คุณต้องการ**อนุญาตภายใต้** คลิก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="b34f4-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="b34f4-115">สําหรับข้อมูลเพิ่มเติม ให้ดู: ["นโยบายไม่อนุญาตให้ให้สิทธิ์ที่ระดับนี้ไปยังผู้รับอย่างน้อยหนึ่งข้อผิดพลาด"เมื่อผู้ใช้พยายามใช้ปฏิทินร่วมกัน](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)</span><span class="sxs-lookup"><span data-stu-id="b34f4-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
