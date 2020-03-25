---
title: การโยกย้าย SharePoint กับ SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931569"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="cf2bf-102">การโยกย้าย SharePoint กับ SPMT</span><span class="sxs-lookup"><span data-stu-id="cf2bf-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="cf2bf-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="cf2bf-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="cf2bf-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="cf2bf-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="cf2bf-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="cf2bf-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="cf2bf-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="cf2bf-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="cf2bf-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="cf2bf-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="cf2bf-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="cf2bf-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="cf2bf-109">**เครื่องมือการโยกย้าย SharePoint**</span><span class="sxs-lookup"><span data-stu-id="cf2bf-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="cf2bf-110">ออกแบบมาเพื่อใช้สําหรับการย้ายตั้งแต่ชุดเล็กที่สุดของไฟล์เพื่อการย้ายองค์กรขนาดใหญ่เครื่องมือการโยกย้าย SharePoint จะช่วยให้คุณสามารถถ่ายโอนข้อมูลของคุณไปยังเมฆและใช้ประโยชน์จากการทํางานร่วมกันใหม่ล่าสุด, ปัญญา, และ โซลูชันการรักษาความปลอดภัยด้วย Office 365</span><span class="sxs-lookup"><span data-stu-id="cf2bf-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="cf2bf-111">ดาวน์โหลด และติดตั้งเครื่องมือการโยกย้าย SharePoint</span><span class="sxs-lookup"><span data-stu-id="cf2bf-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="cf2bf-112">การแก้ไขปัญหาและข้อผิดพลาดของ SPMT ทั่วไป</span><span class="sxs-lookup"><span data-stu-id="cf2bf-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="cf2bf-113">การแก้ไขปัญหาการติดตั้ง SPMT</span><span class="sxs-lookup"><span data-stu-id="cf2bf-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
