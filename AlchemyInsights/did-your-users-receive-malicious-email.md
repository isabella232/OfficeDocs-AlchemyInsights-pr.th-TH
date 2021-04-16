---
title: ผู้ใช้ของคุณได้รับอีเมลที่เป็นอันตราย
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815265"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="e4adf-102">ผู้ใช้ของคุณได้รับอีเมลที่เป็นอันตรายหรือไม่</span><span class="sxs-lookup"><span data-stu-id="e4adf-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="e4adf-103">ขณะนี้คุณสามารถรายงานอีเมลที่เป็นอันตรายไปยังไมโครซอฟท์โดยใช้ การส่ง[โดยผู้ดูแลระบบ ใน ศูนย์&การปฏิบัติตามข้อบังคับ](https://sip.protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="e4adf-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="e4adf-104">ข้อความที่ส่งในการส่ง [ของผู้ดูแลระบบ](https://sip.protection.office.com/reportsubmission) จะถูกสแกน และผลลัพธ์ต่อไปนี้แสดงอยู่ในเมนูป **ลิว** รายละเอียด</span><span class="sxs-lookup"><span data-stu-id="e4adf-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="e4adf-105">ถ้ามีความล้มเหลวในการรับรองความถูกต้องอีเมลของผู้ส่งในเวลาที่จัดส่ง</span><span class="sxs-lookup"><span data-stu-id="e4adf-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="e4adf-106">ข้อมูลเกี่ยวกับความนิยมของนโยบายใดๆ ที่อาจได้รับผลกระทบหรือแทนที่ผลจากข้อความ</span><span class="sxs-lookup"><span data-stu-id="e4adf-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="e4adf-107">ผลลัพธ์การดําเนินการปัจจุบันเพื่อดูว่า URL หรือไฟล์ที่อยู่ในข้อความนั้นเป็นอันตรายหรือไม่</span><span class="sxs-lookup"><span data-stu-id="e4adf-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="e4adf-108">ข้อเสนอแนะจากผู้ให้เกรด</span><span class="sxs-lookup"><span data-stu-id="e4adf-108">Feedback from graders</span></span>

<span data-ttu-id="e4adf-109">ถ้าพบการแทนที่ การ rescan ควรเสร็จสมบูรณ์ในอีกหลายนาที</span><span class="sxs-lookup"><span data-stu-id="e4adf-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="e4adf-110">ถ้าไม่มีปัญหาในการรับรองความถูกต้องทางอีเมลหรือถ้าการส่งอีเมลไม่ได้รับผลกระทบจากการแทนที่ การให้ข้อเสนอแนะจากผู้เกรดอาจใช้เวลาถึงหนึ่งวัน</span><span class="sxs-lookup"><span data-stu-id="e4adf-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="e4adf-111">ถ้าคุณไม่เห็นด้วยกับผลสุดท้ายในข้อความ URL หรือไฟล์ (ถูกบล็อกและไม่ถูกบล็อก) ให้ส่งข้อความอีกครั้งหลังจากผ่านไปหนึ่งวันเพื่อสแกนอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="e4adf-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="e4adf-112">มีโอกาสสูงที่คะแนนจะเปลี่ยนแปลงหลังจากส่งข้อความอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="e4adf-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="e4adf-113">ขณะเดียวกัน คุณสามารถเอาอีเมลที่เป็นอันตรายออกจากกล่องขาเข้าของผู้ใช้ได้โดยการปฏิบัติตามคําแนะ [นํา](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)ในบทความนี้</span><span class="sxs-lookup"><span data-stu-id="e4adf-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="e4adf-114">ลูกค้าที่มี Microsoft Defender for Office 365 สามารถ:</span><span class="sxs-lookup"><span data-stu-id="e4adf-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="e4adf-115">ใช้ [Threat Explorer เพื่อค้นหาและลบอีเมลที่น่าสงสัย](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="e4adf-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="e4adf-116">[ใช้ลิงก์ที่ปลอดภัยเพื่อบล็อก](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) การเข้าถึง URL ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="e4adf-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="e4adf-117">ติดตามผู้ใช้ที่คลิกและเข้าถึง URL ที่เป็นอันตราย:[ดู URL ฟิชชิ่ง และคลิกข้อมูล](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)การค้นหา  &  [Get-UrlTraced](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="e4adf-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="e4adf-118">เริ่ม [การตรวจสอบโดยอัตโนมัติด้วยตนเอง](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="e4adf-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="e4adf-119">คุณยังสามารถป้องกันไฟล์และ URL ที่เป็นอันตรายได้โดยปฏิบัติตามคําแนะนําใน [การป้องกันจาก URL และไฟล์](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="e4adf-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>