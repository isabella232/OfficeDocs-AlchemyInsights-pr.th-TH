---
title: โครงการออนไลน์อยู่ในสถานะอ่านอย่างเดียว
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: dea4e24b0ceb0054f04e6737df0feb761d1143f3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768024"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="fb3cb-102">โครงการออนไลน์อยู่ในสถานะอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="fb3cb-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="fb3cb-103">มีเหตุผลทั่วไปสามประการที่อาจทําให้โครงการออนไลน์ถึงสถานะแบบอ่านอย่างเดียว:</span><span class="sxs-lookup"><span data-stu-id="fb3cb-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="fb3cb-104">องค์กรมีสิทธิ์การใช้งานโครงการออนไลน์ Essentials (s) เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="fb3cb-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="fb3cb-105">นี้ไม่เพียงพอที่จะให้เว็บไซต์มีชีวิตอยู่และในที่สุดก็จะได้รับ de - provisioned</span><span class="sxs-lookup"><span data-stu-id="fb3cb-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="fb3cb-106">เราวางเว็บไซต์ในรัฐอ่านอย่างเดียวเพื่อให้ผู้ดูแลระบบรู้ว่าสิ่งที่ผิดและสามารถได้รับใบอนุญาตที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="fb3cb-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="fb3cb-107">ผู้ดูแลระบบจะต้องเพิ่มสิทธิ์การใช้งาน Project Online Professional และ/หรือ Premium</span><span class="sxs-lookup"><span data-stu-id="fb3cb-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="fb3cb-108">เว็บไซต์จะออกมาจากแบบอ่านอย่างเดียวที่จุดนั้น</span><span class="sxs-lookup"><span data-stu-id="fb3cb-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="fb3cb-109">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[เปรียบเทียบโซลูชันการจัดการโครงการ](https://products.office.com/project/compare-microsoft-project-management-software?tab=1)</span><span class="sxs-lookup"><span data-stu-id="fb3cb-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="fb3cb-110">ถึงโควตาที่กําหนดแล้ว</span><span class="sxs-lookup"><span data-stu-id="fb3cb-110">Assigned quota has been reached.</span></span> <span data-ttu-id="fb3cb-111">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[โควตาโปรแกรมประยุกต์บนเว็บของโครงการ](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota)</span><span class="sxs-lookup"><span data-stu-id="fb3cb-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="fb3cb-112">ตรวจสอบ[การกําหนดค่าค่าสะสมของข้อมูลรายงาน timephased ในโครงการออนไลน์](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online)เพื่อดูว่ารายงาน granularity อาจส่งผลกระทบต่อการใช้งานโควต้า</span><span class="sxs-lookup"><span data-stu-id="fb3cb-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="fb3cb-113">อ่านอย่างเดียวสามารถเป็นเงื่อนไขชั่วคราวมากที่อาจเกิดขึ้นในระหว่างการบํารุงรักษา</span><span class="sxs-lookup"><span data-stu-id="fb3cb-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="fb3cb-114">การบํารุงรักษาส่วนใหญ่ไม่ได้สังเกตเห็นโดยลูกค้าของเราและคุณจะไม่เห็นนี้แต่บางครั้งเมื่อระยะเวลาสั้น ๆ ของการอ่านเท่านั้นมีประสบการณ์</span><span class="sxs-lookup"><span data-stu-id="fb3cb-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
