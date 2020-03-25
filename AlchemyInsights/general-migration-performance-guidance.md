---
title: คําแนะนําเกี่ยวกับประสิทธิภาพการโยกย้ายทั่วไป
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932497"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="34a94-102">คําแนะนําเกี่ยวกับประสิทธิภาพการโยกย้ายทั่วไป</span><span class="sxs-lookup"><span data-stu-id="34a94-102">General migration performance guidance</span></span>

<span data-ttu-id="34a94-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="34a94-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="34a94-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="34a94-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="34a94-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="34a94-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="34a94-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="34a94-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="34a94-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="34a94-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="34a94-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="34a94-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="34a94-109">**คําแนะนําเกี่ยวกับประสิทธิภาพการโยกย้าย**</span><span class="sxs-lookup"><span data-stu-id="34a94-109">**Migration performance guidance**</span></span>

<span data-ttu-id="34a94-110">ประสิทธิภาพการโยกย้ายอาจได้รับผลกระทบจากโครงสร้างพื้นฐานของเครือข่าย ขนาดไฟล์ เวลาการย้าย และการควบคุมปริมาณ</span><span class="sxs-lookup"><span data-stu-id="34a94-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="34a94-111">การทําความเข้าใจสิ่งเหล่านี้จะช่วยให้คุณวางแผนและเพิ่มประสิทธิภาพในการย้ายข้อมูล</span><span class="sxs-lookup"><span data-stu-id="34a94-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="34a94-112">คําแนะนําเกี่ยวกับประสิทธิภาพการโยกย้ายทั่วไป</span><span class="sxs-lookup"><span data-stu-id="34a94-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
