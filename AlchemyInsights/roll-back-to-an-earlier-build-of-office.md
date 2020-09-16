---
title: ย้อนกลับไปยังรุ่นก่อนหน้าของ Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1741"
- "9000140"
ms.openlocfilehash: 9f6a812def2b46bf32d836781d0336aea5ba3ed1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727838"
---
# <a name="roll-back-to-an-earlier-build-of-office"></a><span data-ttu-id="be35b-102">ย้อนกลับไปยังรุ่นก่อนหน้าของ Office</span><span class="sxs-lookup"><span data-stu-id="be35b-102">Roll back to an earlier build of Office</span></span>

<span data-ttu-id="be35b-103">เมื่อต้องการย้อนกลับไปยังรุ่นของแอป Microsoft ๓๖๕เวอร์ชันก่อนหน้าให้ดูที่[วิธีการแปลงกลับเป็น Office เวอร์ชันก่อนหน้า](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic)</span><span class="sxs-lookup"><span data-stu-id="be35b-103">To revert to an earlier Microsoft 365 Apps build or version, see [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic).</span></span> <span data-ttu-id="be35b-104">เมื่อต้องการสลับจากการสมัครใช้งาน Microsoft ๓๖๕หนึ่งไปยังอีกบัญชีหนึ่งให้ดูที่[สลับไปยังแผน microsoft ๓๖๕สำหรับธุรกิจอื่น](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="be35b-104">To switch from one Microsoft 365 subscription to another, see  [Switch to a different Microsoft 365 for business plan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>

- <span data-ttu-id="be35b-105">เมื่อต้องการค้นหาเวอร์ชันของ Office ที่คุณกำลังใช้งานอยู่ให้ดู [เกี่ยวกับ office: ฉันกำลังใช้ office เวอร์ชันใด](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19)อยู่</span><span class="sxs-lookup"><span data-stu-id="be35b-105">To find the version of Office you are currently using, see [About Office: What version of Office am I using?](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19).</span></span>
- <span data-ttu-id="be35b-106">เมื่อต้องการกำหนดรุ่นที่คุณต้องการย้อนกลับไปให้ดู[ประวัติการอัปเดตสำหรับแอป Microsoft ๓๖๕ (แสดงตามวันที่)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7)</span><span class="sxs-lookup"><span data-stu-id="be35b-106">To determine the build you want to roll back to, see [Update history for Microsoft 365 Apps (listed by date)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7).</span></span>
- <span data-ttu-id="be35b-107">กำหนดค่าการตั้งค่า**TargetVersion**เพื่อแปลงกลับไปเป็นรุ่นก่อนหน้าโดยใช้[วิธีการแปลงกลับไปเป็นเวอร์ชันก่อนหน้าของ Office หรือการ](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic)[หน่วงเวลาที่ได้รับการปรับปรุงฟีเจอร์จากแชนเนลแบบครึ่งปีเมื่อใช้เครือข่ายการนำส่งเนื้อหาของ office (CDN)](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn)</span><span class="sxs-lookup"><span data-stu-id="be35b-107">Configure the **TargetVersion** setting to revert to the earlier build by using [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic) or [Delay receiving feature updates from Semi-Annual Channel when using the Office Content Delivery Network (CDN)](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn).</span></span></br>
    <span data-ttu-id="be35b-108">เมื่อมีการตั้งค่าเวอร์ชันเป้าหมายการอัปเดต Office ไปยังเวอร์ชันนั้นในครั้งต่อไปที่ค้นหาการอัปเดต</span><span class="sxs-lookup"><span data-stu-id="be35b-108">When the target version is set, Office updates to that version the next time it looks for updates.</span></span>