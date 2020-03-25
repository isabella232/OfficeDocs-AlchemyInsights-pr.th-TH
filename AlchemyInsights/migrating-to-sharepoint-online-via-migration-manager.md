---
title: กําลังย้ายข้อมูลไปยัง SharePoint แบบออนไลน์ผ่านทางโปรแกรมจัดการการโยกย้าย
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
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932375"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="ff699-102">กําลังย้ายข้อมูลไปยัง SharePoint แบบออนไลน์ผ่านทางโปรแกรมจัดการการโยกย้าย</span><span class="sxs-lookup"><span data-stu-id="ff699-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="ff699-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="ff699-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ff699-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="ff699-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ff699-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="ff699-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ff699-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="ff699-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ff699-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="ff699-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ff699-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="ff699-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ff699-109">**ตัวจัดการการย้าย**</span><span class="sxs-lookup"><span data-stu-id="ff699-109">**Migration Manager**</span></span>

<span data-ttu-id="ff699-110">ตัวจัดการการย้ายจะแนะนําคุณผ่านการตั้งค่าไคลเอ็นต์และการสร้างงานของคุณ</span><span class="sxs-lookup"><span data-stu-id="ff699-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="ff699-111">คุณสามารถระบุการตั้งค่าส่วนกลางหรือระดับงาน</span><span class="sxs-lookup"><span data-stu-id="ff699-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="ff699-112">เริ่มต้นใช้งานตัวจัดการการย้าย</span><span class="sxs-lookup"><span data-stu-id="ff699-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="ff699-113">ตั้งค่าไคลเอ็นต์ตัวจัดการการย้าย</span><span class="sxs-lookup"><span data-stu-id="ff699-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="ff699-114">การตั้งค่าตัวจัดการการย้าย</span><span class="sxs-lookup"><span data-stu-id="ff699-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
