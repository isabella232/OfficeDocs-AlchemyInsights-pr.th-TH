---
title: การแก้ไขปัญหาเหตุการณ์จากอีเมล
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658753"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="84d9a-102">การแก้ไขปัญหาเหตุการณ์จากอีเมล</span><span class="sxs-lookup"><span data-stu-id="84d9a-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="84d9a-103">ตรวจสอบว่าฟีเจอร์ถูกเปิดใช้งานสำหรับกล่องจดหมาย:**รับ <mailbox> -EventsFromEmailConfiguration-ข้อมูลประจำตัว**</span><span class="sxs-lookup"><span data-stu-id="84d9a-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="84d9a-104">จากนั้นให้ดูที่ "เหตุการณ์จากอีเมล" บันทึกการ **ส่งออก-MailboxDiagnosticLogs <mailbox> -คอมโพเนนต์ TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="84d9a-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="84d9a-105">ในบันทึก "เหตุการณ์จากอีเมล" ให้ค้นหา InternetMessageId ที่ตรงกับรายการในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="84d9a-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="84d9a-106">TrustScore จะกำหนดว่ารายการนั้นถูกเพิ่มหรือไม่</span><span class="sxs-lookup"><span data-stu-id="84d9a-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="84d9a-107">เหตุการณ์จะถูกเพิ่มถ้า TrustScore = "เชื่อถือได้"</span><span class="sxs-lookup"><span data-stu-id="84d9a-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="84d9a-108">TrustScore จะถูกกำหนดโดย SPF, Dkim หรือคุณสมบัติ Dmarc ซึ่งอยู่ในส่วนหัวของข้อความ</span><span class="sxs-lookup"><span data-stu-id="84d9a-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="84d9a-109">เมื่อต้องการดูคุณสมบัติเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="84d9a-109">To view these properties:</span></span>

<span data-ttu-id="84d9a-110">**Outlook บนเดสก์ท็อป**</span><span class="sxs-lookup"><span data-stu-id="84d9a-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="84d9a-111">เปิดรายการ</span><span class="sxs-lookup"><span data-stu-id="84d9a-111">Open the item</span></span>
- <span data-ttu-id="84d9a-112">ไฟล์-คุณสมบัติ >-ส่วนหัวของอินเทอร์เน็ต ></span><span class="sxs-lookup"><span data-stu-id="84d9a-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="84d9a-113">หรือ</span><span class="sxs-lookup"><span data-stu-id="84d9a-113">or</span></span>

<span data-ttu-id="84d9a-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="84d9a-114">**MFCMapi**</span></span>

- <span data-ttu-id="84d9a-115">นำทางไปยังรายการในกล่องจดหมายเข้า</span><span class="sxs-lookup"><span data-stu-id="84d9a-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="84d9a-116">ค้นหา PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="84d9a-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="84d9a-117">คุณสมบัติเหล่านี้จะถูกกำหนดและบันทึกในระหว่างการขนส่งและเส้นทาง</span><span class="sxs-lookup"><span data-stu-id="84d9a-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="84d9a-118">สำหรับการแก้ไขปัญหาเพิ่มเติมคุณอาจต้องติดตามการสนับสนุนการขนส่งเกี่ยวกับความล้มเหลวใน SPF, DKIM และ. หรือ DMARC</span><span class="sxs-lookup"><span data-stu-id="84d9a-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>