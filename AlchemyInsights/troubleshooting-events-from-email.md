---
title: การแก้ไขปัญหากิจกรรมจากอีเมล
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834858"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="3c43d-102">การแก้ไขปัญหากิจกรรมจากอีเมล</span><span class="sxs-lookup"><span data-stu-id="3c43d-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="3c43d-103">ตรวจสอบว่ามีการเปิดใช้งานฟีเจอร์นี้กับกล่องจดหมายหรือไม่ **: Get-EventsFromAmailConfiguration <mailbox> -Identity**</span><span class="sxs-lookup"><span data-stu-id="3c43d-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="3c43d-104">จากนั้นดูที่บันทึก 'เหตุการณ์จากอีเมล' **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="3c43d-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="3c43d-105">ในบันทึก 'กิจกรรมจากอีเมล' ให้ค้นหา InternetMessageId ที่ตรงกับรายการในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="3c43d-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="3c43d-106">TrustScore จะระบุว่ารายการถูกเพิ่มหรือไม่</span><span class="sxs-lookup"><span data-stu-id="3c43d-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="3c43d-107">เหตุการณ์จะถูกเพิ่มถ้า TrustScore = "Trusted" เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="3c43d-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="3c43d-108">TrustScore จะถูกกําหนดโดยคุณสมบัติ SPF, Dkim หรือ Dmarc ซึ่งอยู่ในส่วนหัวของข้อความ</span><span class="sxs-lookup"><span data-stu-id="3c43d-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="3c43d-109">เมื่อต้องการดูคุณสมบัติเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="3c43d-109">To view these properties:</span></span>

<span data-ttu-id="3c43d-110">**Outlook บนเดสก์ท็อป**</span><span class="sxs-lookup"><span data-stu-id="3c43d-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="3c43d-111">เปิดรายการ</span><span class="sxs-lookup"><span data-stu-id="3c43d-111">Open the item</span></span>
- <span data-ttu-id="3c43d-112">File -> Properties ->ส่วนหัวอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="3c43d-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="3c43d-113">หรือ</span><span class="sxs-lookup"><span data-stu-id="3c43d-113">or</span></span>

<span data-ttu-id="3c43d-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="3c43d-114">**MFCMapi**</span></span>

- <span data-ttu-id="3c43d-115">นําทางไปยังรายการในกล่องจดหมายเข้า</span><span class="sxs-lookup"><span data-stu-id="3c43d-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="3c43d-116">ค้นหาPR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="3c43d-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="3c43d-117">คุณสมบัติเหล่านี้จะถูกกําหนดและบันทึกระหว่างการส่งผ่านและการกําหนดเส้นทาง</span><span class="sxs-lookup"><span data-stu-id="3c43d-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="3c43d-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in SPF, DKIM and.or DMARC.</span><span class="sxs-lookup"><span data-stu-id="3c43d-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>