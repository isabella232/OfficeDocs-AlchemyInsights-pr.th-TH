---
title: เคล็ดลับนโยบาย DLP ไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932605"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="6849e-102">ปัญหาคําแนะนํานโยบาย DLP</span><span class="sxs-lookup"><span data-stu-id="6849e-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="6849e-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="6849e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6849e-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="6849e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6849e-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="6849e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6849e-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="6849e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6849e-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="6849e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6849e-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="6849e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="6849e-109">**เคล็ดลับนโยบาย DLP**</span><span class="sxs-lookup"><span data-stu-id="6849e-109">**DLP policy tips**</span></span>

<span data-ttu-id="6849e-110">เมื่อใช้**นโยบาย DLP**ผู้ใช้จะได้รับการแจ้งเตือนเกี่ยวกับการละเมิดนโยบายด้วย**เคล็ดลับนโยบาย**</span><span class="sxs-lookup"><span data-stu-id="6849e-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="6849e-111">ผู้ดูแลระบบสามารถกําหนดค่าคําแนะนํานโยบายให้แสดงขณะทดสอบนโยบาย DLP ของตน หรือเมื่อนโยบายอยู่ในโหมดการบังคับใช้แบบเต็ม</span><span class="sxs-lookup"><span data-stu-id="6849e-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="6849e-112">เมื่อต้องการกําหนดค่านโยบายเคล็ดลับนโยบายนโยบาย DLP ของคุณในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามกฎระเบียบในโหมดการบังคับใช้แบบเต็ม ให้ทําดังนี้</span><span class="sxs-lookup"><span data-stu-id="6849e-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="6849e-113">ตรวจสอบให้แน่ใจว่าได้**เปิดใช้งาน**เคล็ดลับนโยบายในกฎ DLP โดยใช้ขั้นตอน[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="6849e-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="6849e-114">ตรวจสอบให้แน่ใจ**ว่าเนื้อหาของคุณตรงกับ\*\*\*\*สิ่งที่จําเป็น**เพื่อทริกเกอร์กฎที่กล่าวถึงในบทความนี้[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="6849e-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="6849e-115">คําแนะนํานโยบายแสดงทั้งใน OWA และ Outlook</span><span class="sxs-lookup"><span data-stu-id="6849e-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="6849e-116">อย่างไรก็ตาม เมื่อใช้**Outlook 2013 หรือรุ่นที่ใหม่กว่า**</span><span class="sxs-lookup"><span data-stu-id="6849e-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="6849e-117">เงื่อนไขเหล่านี้จะแสดงอยู่ที่นี่:[เงื่อนไขที่ได้รับการสนับสนุนสําหรับ Outlook 2013 หรือรุ่นที่ใหม่กว่าสําหรับการแสดงคําแนะนํานโยบาย](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="6849e-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="6849e-118">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับเคล็ดลับนโยบาย DLP ให้ดูที่:[แสดงเคล็ดลับนโยบายสําหรับนโยบาย DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="6849e-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  