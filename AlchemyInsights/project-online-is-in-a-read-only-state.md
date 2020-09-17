---
title: Project Online อยู่ในสถานะแบบอ่านอย่างเดียว
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: ad2a9f95bf30708772edb166945f3f42e0f1f503
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801671"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="813cf-102">Project Online อยู่ในสถานะแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="813cf-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="813cf-103">มีสาเหตุทั่วไปสามประการที่ทำให้ Project Online สามารถเข้าถึงสถานะแบบอ่านอย่างเดียวได้:</span><span class="sxs-lookup"><span data-stu-id="813cf-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="813cf-104">องค์กรมีการให้สิทธิ์การใช้งานสิ่งจำเป็นสำหรับ Project Online เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="813cf-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="813cf-105">นี่ไม่เพียงพอที่จะทำให้ไซต์มีชีวิตอยู่และในที่สุดจะได้รับการเตรียมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="813cf-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="813cf-106">เราวางไซต์ในสถานะแบบอ่านอย่างเดียวเพื่อให้ผู้ดูแลระบบทราบว่ามีบางสิ่งผิดปกติและสามารถรับสิทธิ์การใช้งานที่ถูกต้องได้</span><span class="sxs-lookup"><span data-stu-id="813cf-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="813cf-107">ผู้ดูแลระบบจะต้องเพิ่มสิทธิ์การใช้งาน Project Online และ/หรือสิทธิ์การใช้งานพิเศษ</span><span class="sxs-lookup"><span data-stu-id="813cf-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="813cf-108">ไซต์จะออกจากแบบอ่านอย่างเดียวที่จุดนั้น</span><span class="sxs-lookup"><span data-stu-id="813cf-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="813cf-109">สำหรับข้อมูลเพิ่มเติมให้ดูที่[เปรียบเทียบโซลูชันการจัดการโครงการ](https://products.office.com/project/compare-microsoft-project-management-software?tab=1)</span><span class="sxs-lookup"><span data-stu-id="813cf-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="813cf-110">มีการเข้าถึงโควตาที่ได้รับมอบหมายแล้ว</span><span class="sxs-lookup"><span data-stu-id="813cf-110">Assigned quota has been reached.</span></span> <span data-ttu-id="813cf-111">สำหรับข้อมูลเพิ่มเติมให้ดูที่[โควตาของ Project Web App](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota)</span><span class="sxs-lookup"><span data-stu-id="813cf-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="813cf-112">ตรวจสอบการ [กำหนดค่าสะสมของข้อมูลการรายงานจเข้าใน Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) เพื่อดูว่าองค์ประกอบของรายงานอาจส่งผลกระทบต่อการใช้งานโควตาอย่างไร</span><span class="sxs-lookup"><span data-stu-id="813cf-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="813cf-113">แบบอ่านอย่างเดียวอาจเป็นเงื่อนไขชั่วคราวที่อาจเกิดขึ้นในระหว่างการบำรุงรักษา</span><span class="sxs-lookup"><span data-stu-id="813cf-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="813cf-114">การบำรุงรักษาส่วนใหญ่จะไม่ได้รับการสังเกตเห็นโดยลูกค้าของเราและคุณจะไม่เห็นสิ่งนี้แต่จะมีบางครั้งที่มีการใช้งานแบบอ่านอย่างเดียวในช่วงเวลาสั้นๆ</span><span class="sxs-lookup"><span data-stu-id="813cf-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
