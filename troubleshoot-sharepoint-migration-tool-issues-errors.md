---
title: การแก้ไขปัญหาเครื่องมือการโยกย้าย SharePoint และข้อผิดพลาด
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931137"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="73a4c-102">การแก้ไขปัญหาเครื่องมือการโยกย้าย SharePoint และข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="73a4c-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="73a4c-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="73a4c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="73a4c-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="73a4c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="73a4c-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="73a4c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="73a4c-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="73a4c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="73a4c-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="73a4c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="73a4c-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="73a4c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="73a4c-109">**ปัญหาทั่วไปและข้อผิดพลาด**</span><span class="sxs-lookup"><span data-stu-id="73a4c-109">**Common issues and errors**</span></span>

<span data-ttu-id="73a4c-110">คุณอาจพบปัญหาทั่วไปและข้อผิดพลาดบางอย่างเมื่อใช้เครื่องมือการโยกย้าย SharePoint (SPMT)</span><span class="sxs-lookup"><span data-stu-id="73a4c-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="73a4c-111">โปรดอ้างอิงลิงก์ด้านล่างสําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="73a4c-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="73a4c-112">การแก้ไขปัญหาและข้อผิดพลาดของ SPMT ทั่วไป</span><span class="sxs-lookup"><span data-stu-id="73a4c-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="73a4c-113">การแก้ไขปัญหาการติดตั้ง SPMT</span><span class="sxs-lookup"><span data-stu-id="73a4c-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)