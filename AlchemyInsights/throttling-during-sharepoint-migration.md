---
title: การควบคุมปริมาณในระหว่างการโยกย้าย SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "9000353"
- "1987"
- "9000136"
- "2968"
ms.assetid: ''
ms.openlocfilehash: dc77c462fcf32817c92709852e2d03ab2086b9a4
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958917"
---
# <a name="sharepoint-throttling"></a><span data-ttu-id="d3be5-102">การควบคุมปริมาณ SharePoint</span><span class="sxs-lookup"><span data-stu-id="d3be5-102">SharePoint throttling</span></span>

<span data-ttu-id="d3be5-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="d3be5-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d3be5-104">**การควบคุมปริมาณแบบออนไลน์ของ SharePoint**</span><span class="sxs-lookup"><span data-stu-id="d3be5-104">**SharePoint Online throttling**</span></span>

<span data-ttu-id="d3be5-105">SharePoint Online ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพสูงสุดและความน่าเชื่อถือของบริการ SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="d3be5-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="d3be5-106">การควบคุมปริมาณ จํากัด จํานวนของการกระทําของผู้ใช้หรือเรียกพร้อมกัน (ตามสคริปต์หรือรหัส) เพื่อป้องกันการใช้ทรัพยากรมากเกินไป</span><span class="sxs-lookup"><span data-stu-id="d3be5-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span>

<span data-ttu-id="d3be5-107">สําหรับข้อมูลเพิ่มเติมกรุณาเยี่ยมชมลิงค์ด้านล่าง:</span><span class="sxs-lookup"><span data-stu-id="d3be5-107">For more information please visit the links below:</span></span>

- [<span data-ttu-id="d3be5-108">หลีกเลี่ยงการถูกควบคุมปริมาณหรือถูกบล็อกใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="d3be5-108">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)
- [<span data-ttu-id="d3be5-109">การย้ายข้อมูลและการควบคุมปริมาณ SPO</span><span class="sxs-lookup"><span data-stu-id="d3be5-109">Data Migration and SPO Throttling</span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)
- [<span data-ttu-id="d3be5-110">ออนไลน์และ OneDrive ความเร็วในการโยกย้าย</span><span class="sxs-lookup"><span data-stu-id="d3be5-110">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
- [<span data-ttu-id="d3be5-111">จัดการการควบคุมปริมาณ SharePoint แบบออนไลน์ โดยใช้กลับชี้แจงออก</span><span class="sxs-lookup"><span data-stu-id="d3be5-111">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)
- [<span data-ttu-id="d3be5-112">การวางแผนกําลังการผลิตและการทดสอบโหลด SharePoint ออนไลน์</span><span class="sxs-lookup"><span data-stu-id="d3be5-112">Capacity planning and load testing SharePoint Online</span></span>](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0)
- [<span data-ttu-id="d3be5-113">ฉันประสบประสิทธิภาพการทํางานที่ไม่ดีหรือการควบคุมปริมาณในระหว่างการย้าย</span><span class="sxs-lookup"><span data-stu-id="d3be5-113">I am experiencing poor performance or throttling during migration</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed#faq-and-troubleshooting)