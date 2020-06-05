---
title: การแก้ไขปัญหาเหตุการณ์จากอีเมล
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569401"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="b88c0-102">การแก้ไขปัญหาเหตุการณ์จากอีเมล</span><span class="sxs-lookup"><span data-stu-id="b88c0-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="b88c0-103">ตรวจสอบลักษณะการทํางานถูกเปิดใช้งานสําหรับกล่องจดหมาย:\*\*รับเหตุการณ์From-อีเมลการกําหนดค่า-รหัสประจําตัว <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="b88c0-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="b88c0-104">แล้วดูที่ 'เหตุการณ์จากอีเมล' บันทึก**การส่งออก MailboxDiagnosticLogs <mailbox> -เวลาคอมโพเนนต์Profile**</span><span class="sxs-lookup"><span data-stu-id="b88c0-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="b88c0-105">ในบันทึก 'เหตุการณ์จากอีเมล' ให้ค้นหา InternetMessageId ที่ตรงกับรายการในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="b88c0-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="b88c0-106">TrustScore จะกําหนดว่ารายการนั้นถูกเพิ่มหรือไม่</span><span class="sxs-lookup"><span data-stu-id="b88c0-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="b88c0-107">เหตุการณ์จะถูกเพิ่มเฉพาะเมื่อ TrustScore = "เชื่อถือ"</span><span class="sxs-lookup"><span data-stu-id="b88c0-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="b88c0-108">คุณสมบัติ Dm หรือ Dmarc ซึ่งอยู่ในส่วนหัวของข้อความ</span><span class="sxs-lookup"><span data-stu-id="b88c0-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="b88c0-109">เมื่อต้องการดูคุณสมบัติเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="b88c0-109">To view these properties:</span></span>

<span data-ttu-id="b88c0-110">**มุมมองเดสก์ท็อป**</span><span class="sxs-lookup"><span data-stu-id="b88c0-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="b88c0-111">เปิดรายการ</span><span class="sxs-lookup"><span data-stu-id="b88c0-111">Open the item</span></span>
- <span data-ttu-id="b88c0-112">แฟ้ม -> คุณสมบัติ -> ส่วนหัวอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="b88c0-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="b88c0-113">หรือ</span><span class="sxs-lookup"><span data-stu-id="b88c0-113">or</span></span>

<span data-ttu-id="b88c0-114">**Mfcmapi**</span><span class="sxs-lookup"><span data-stu-id="b88c0-114">**MFCMapi**</span></span>

- <span data-ttu-id="b88c0-115">นําทางไปยังรายการในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="b88c0-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="b88c0-116">มองหาPR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="b88c0-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="b88c0-117">คุณสมบัติเหล่านี้จะถูกกําหนด และบันทึกในระหว่างการขนส่งและสายงานการผลิต</span><span class="sxs-lookup"><span data-stu-id="b88c0-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="b88c0-118">สําหรับการแก้ไขปัญหาเพิ่มเติม คุณอาจต้องติดตามด้วยการสนับสนุนการขนส่งเกี่ยวกับความล้มเหลวใน SPF, DKIM และ DMARC</span><span class="sxs-lookup"><span data-stu-id="b88c0-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>