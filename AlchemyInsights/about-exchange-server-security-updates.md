---
title: เกี่ยวกับการอัปเดตความปลอดภัยของ Exchange Server
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482985"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="e6f72-102">เกี่ยวกับการอัปเดตความปลอดภัยของ Exchange Server</span><span class="sxs-lookup"><span data-stu-id="e6f72-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="e6f72-103">Microsoft ได้เผยแพร่ชุดการอัปเดตความปลอดภัยที่วิกฤติใน Exchange Server ภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="e6f72-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="e6f72-104">เวอร์ชันของเซิร์ฟเวอร์ที่ได้รับผลกระทบคือระดับการอัปเดตใดๆ ของ Exchange Server 2010, 2013, 2016 และ 2019</span><span class="sxs-lookup"><span data-stu-id="e6f72-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="e6f72-105">Exchange Online จะไม่ได้รับผลกระทบ แต่ถ้าคุณมีเซิร์ฟเวอร์ Exchange ภายในองค์กรบางส่วนเนื่องจากการกําหนดค่าแบบไฮบริด เซิร์ฟเวอร์เหล่านั้นอาจมีความเสี่ยง</span><span class="sxs-lookup"><span data-stu-id="e6f72-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="e6f72-106">เมื่อต้องการอัปเดตเซิร์ฟเวอร์ภายในองค์กรของคุณจะต้องใช้งาน Exchange เวอร์ชันต่อไปนี้เป็นอย่างน้อย:</span><span class="sxs-lookup"><span data-stu-id="e6f72-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="e6f72-107">Exchange 2010 Service Pack 3</span><span class="sxs-lookup"><span data-stu-id="e6f72-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="e6f72-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="e6f72-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="e6f72-109">Exchange Server 2016 CU 19 หรือ CU 18</span><span class="sxs-lookup"><span data-stu-id="e6f72-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="e6f72-110">Exchange Server 2019 CU 8 หรือ CU 7</span><span class="sxs-lookup"><span data-stu-id="e6f72-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="e6f72-111">โปรดดูประกาศต่อไปนี้เกี่ยวกับสถานที่ตั้งของการแก้ไข: [เผยแพร่แล้ว: การอัปเดตความปลอดภัยของ Exchange Server ในเดือนมีนาคม 2021](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="e6f72-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="e6f72-112">**หมายเหตุสําคัญ:**</span><span class="sxs-lookup"><span data-stu-id="e6f72-112">**Important notes:**</span></span>

<span data-ttu-id="e6f72-113">การติดตั้งการอัปเดตจะใช้งานไม่ได้ถ้าเซิร์ฟเวอร์ภายในองค์กรของคุณไม่ได้ใช้ Exchange เวอร์ชันที่ต้องใช้ ตามรายการข้างต้น</span><span class="sxs-lookup"><span data-stu-id="e6f72-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="e6f72-114">ถ้าติดตั้งการอัปเดตด้วยตนเอง โปรดอ่านส่วน "ปัญหาที่ทราบแล้ว" ของการอัปเดตบทความ KB เพื่อดูข้อมูลสําคัญ</span><span class="sxs-lookup"><span data-stu-id="e6f72-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="e6f72-115">การอัปเดตการรักษาความปลอดภัยต้องเรียกใช้จากพร้อมท์ CMD/PowerShell ด้วยสิทธิ์ผู้ดูแล!</span><span class="sxs-lookup"><span data-stu-id="e6f72-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
