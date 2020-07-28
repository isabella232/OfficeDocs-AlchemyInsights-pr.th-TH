---
title: ย้อนกลับไปยังการสร้าง Office ก่อนหน้านี้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1741"
- "9000140"
ms.openlocfilehash: 8c7d019ec1aa6c26cffebbcd2c3e5751c853e3a4
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440320"
---
# <a name="roll-back-to-an-earlier-build-of-office"></a><span data-ttu-id="73e08-102">ย้อนกลับไปยังการสร้าง Office ก่อนหน้านี้</span><span class="sxs-lookup"><span data-stu-id="73e08-102">Roll back to an earlier build of Office</span></span>

<span data-ttu-id="73e08-103">เมื่อต้องการแปลงกลับเป็นรุ่นหรือเวอร์ชันของแอป Microsoft 365 รุ่นก่อนหน้า ให้ดูที่[วิธีการแปลงกลับไปเป็น Office รุ่นก่อนหน้านี้](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic)</span><span class="sxs-lookup"><span data-stu-id="73e08-103">To revert to an earlier Microsoft 365 Apps build or version, see [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic).</span></span> <span data-ttu-id="73e08-104">เมื่อต้องการสลับจากการสมัครใช้งาน Microsoft 365 หนึ่งไปยังอีกราย ให้ดูที่[สลับไปยังแผน Microsoft 365 สําหรับธุรกิจแผนอื่น](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="73e08-104">To switch from one Microsoft 365 subscription to another, see  [Switch to a different Microsoft 365 for business plan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>

- <span data-ttu-id="73e08-105">เมื่อต้องการค้นหารุ่นของ Office ที่คุณใช้อยู่ในปัจจุบัน ให้ดูที่[เกี่ยวกับ Office: ฉันกําลังใช้ Office เวอร์ชันใด](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19)อยู่</span><span class="sxs-lookup"><span data-stu-id="73e08-105">To find the version of Office you are currently using, see [About Office: What version of Office am I using?](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19).</span></span>
- <span data-ttu-id="73e08-106">เมื่อต้องการกําหนดการสร้างที่คุณต้องการย้อนกลับไปที่ ดู[ประวัติการปรับปรุงสําหรับแอป Microsoft 365 (แสดงรายการตามวันที่)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7)</span><span class="sxs-lookup"><span data-stu-id="73e08-106">To determine the build you want to roll back to, see [Update history for Microsoft 365 Apps (listed by date)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7).</span></span>
- <span data-ttu-id="73e08-107">กําหนดค่าการตั้งค่า**TargetVersion**เพื่อแปลงกลับไปเป็นรุ่นก่อนหน้านี้ โดยใช้[วิธีการแปลงกลับไปเป็น Office รุ่นก่อนหน้านี้](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic)หรือ[ความล่าช้าที่ได้รับการปรับปรุงคุณลักษณะจากช่องสัญญาณกึ่งปีเมื่อใช้ Office เนื้อหาการจัดส่งเครือข่าย (CDN)](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn)</span><span class="sxs-lookup"><span data-stu-id="73e08-107">Configure the **TargetVersion** setting to revert to the earlier build by using [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic) or [Delay receiving feature updates from Semi-Annual Channel when using the Office Content Delivery Network (CDN)](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn).</span></span></br>
    <span data-ttu-id="73e08-108">เมื่อมีการตั้งค่ารุ่นเป้าหมาย Office จะอัปเดตเวอร์ชันนั้นในครั้งต่อไปที่ค้นหาการปรับปรุง</span><span class="sxs-lookup"><span data-stu-id="73e08-108">When the target version is set, Office updates to that version the next time it looks for updates.</span></span>