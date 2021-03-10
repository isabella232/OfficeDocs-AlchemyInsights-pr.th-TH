---
title: ค้นหาไซต์
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694555"
---
# <a name="do-site-discovery"></a><span data-ttu-id="6e042-102">ค้นหาไซต์</span><span class="sxs-lookup"><span data-stu-id="6e042-102">Do site discovery</span></span>

<span data-ttu-id="6e042-103">ถ้าองค์กรของคุณยังคงใช้แอปพลิเคชันบนเว็บดั้งเดิมและแผนเพื่อใช้โหมด Internet Explorer (ซึ่งลูกค้าส่วนใหญ่ใช้) คุณควรค้นหาไซต์เพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="6e042-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="6e042-104">**คุณได้ปรับใช้ Microsoft Edge เวอร์ชันที่เก่ากว่าแล้ว**</span><span class="sxs-lookup"><span data-stu-id="6e042-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="6e042-105">ถ้าคุณได้กําหนดค่ารายการไซต์องค์กรให้ใช้งานกับ Microsoft Edge เวอร์ชันดั้งเดิมแล้ว การค้นพบไซต์ของคุณเกือบเสร็จสิ้นแล้ว</span><span class="sxs-lookup"><span data-stu-id="6e042-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="6e042-106">สิ่งหนึ่งที่คุณอาจต้องใช้คือการเพิ่มไซต์ที่เป็นกลาง</span><span class="sxs-lookup"><span data-stu-id="6e042-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="6e042-107">ไซต์ที่เป็นกลางคือไซต์ที่ให้การลงชื่อเข้าระบบครั้งเดียว (SSO)</span><span class="sxs-lookup"><span data-stu-id="6e042-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="6e042-108">ถ้าคุณไปที่ไซต์ที่เป็นกลางจาก Microsoft Edge คุณต้องการอยู่ใน Microsoft Edge เพื่อรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="6e042-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="6e042-109">ถ้าคุณไปยังไซต์ที่เป็นกลางในโหมด Internet Explorer คุณต้องการอยู่ในโหมด Internet Explorer เพื่อรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="6e042-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="6e042-110">ระบุ SSO หรือไซต์ที่เป็นกลางอื่นๆ ที่คุณใช้และเพิ่มไซต์เหล่านี้ลงในรายการไซต์องค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="6e042-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="6e042-111">**Internet Explorer เป็นเบราว์เซอร์เริ่มต้นของคุณ**</span><span class="sxs-lookup"><span data-stu-id="6e042-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="6e042-112">ถ้าคุณแค่ใช้ Internet Explorer ในตอนนี้ คุณอาจไม่ทราบว่าไซต์ใดได้รับการอัปเกรดเป็นมาตรฐานเว็บสมัยใหม่ และยังคงต้องการ Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="6e042-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="6e042-113">คุณจะต้องค้นหาและเพิ่มไซต์เหล่านี้ลงในรายการไซต์ขององค์กรเพื่อให้คุณสามารถใช้โหมด Internet Explorer ได้เฉพาะกับไซต์เหล่านั้นเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="6e042-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="6e042-114">[การค้นพบไซต์องค์กร](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) จะค้นพบไซต์ที่อาจต้องใช้โหมด Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="6e042-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="6e042-115">โดยสามารถรวบรวมข้อมูลบนคอมพิวเตอร์ที่ใช้ Windows Internet Explorer 8 ผ่าน Internet Explorer 11 บน Windows 10, Windows 8.1 หรือ Windows 7</span><span class="sxs-lookup"><span data-stu-id="6e042-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="6e042-116">**วิเคราะห์ข้อมูล**</span><span class="sxs-lookup"><span data-stu-id="6e042-116">**Analyze the data**</span></span>

<span data-ttu-id="6e042-117">หลังจากที่คุณรวบรวมข้อมูลไซต์ เราขอแนะนนะให้กระบวนการสี่ขั้นตอนต่อไปนี้วิเคราะห์ข้อมูล:</span><span class="sxs-lookup"><span data-stu-id="6e042-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="6e042-118">เรียงล>บข้อมูลตามโดเมน ตามด้วย URL</span><span class="sxs-lookup"><span data-stu-id="6e042-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="6e042-119">กําหนดขอบเขตของแอปเพื่อกําหนดค่าโหมด Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="6e042-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="6e042-120">คุณต้องการรวมไซต์และตัวควบคุมเว็บทั้งหมดที่กําหนดแอป แต่คุณไม่ต้องรวมไซต์และตัวควบคุมเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="6e042-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="6e042-121">บางไซต์อาจง่ายเหมือนกับ *https://contoso.com/app1* ที่ผู้อื่นอาจต้องการให้คุณกําหนดหลายไซต์และหน้า</span><span class="sxs-lookup"><span data-stu-id="6e042-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="6e042-122">ทดสอบแอปเพื่อตรวจสอบว่าแอปไม่สามารถใช้งานภาษาดั้งเดิมได้</span><span class="sxs-lookup"><span data-stu-id="6e042-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="6e042-123">ไซต์มากมายจะเสนอเนื้อหาที่ทันสมัยเมื่อพวกเขาตรวจพบเบราว์เซอร์ที่ทันสมัย และมีเฉพาะเนื้อหาดั้งเดิมเมื่อตรวจพบ Internet Explorer เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="6e042-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="6e042-124">เพิ่มแอปลงในรายการไซต์องค์กรของคุณถ้าการทดสอบล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="6e042-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="6e042-125">แนวทางปฏิบัติที่ดีที่สุดคือ จัดกลุ่มไซต์ทั้งหมดที่ประกอบเป็นแอป</span><span class="sxs-lookup"><span data-stu-id="6e042-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="6e042-126">ด้วยวิธีนี้ เมื่อคุณอัปเกรดแอป การเอาทั้งไซต์ออกจากโหมด Internet Explorer จะง่ายขึ้นและเริ่มใช้เบราว์เซอร์ที่ทันสมัยของแอปนั้น</span><span class="sxs-lookup"><span data-stu-id="6e042-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="6e042-127">เมื่อคุณค้นหาไซต์เสร็จแล้ว และคุณได้วิเคราะห์ข้อมูล คุณก็พร้อมที่จะเริ่มดูกลยุทธ์แชนเนลของคุณแล้ว</span><span class="sxs-lookup"><span data-stu-id="6e042-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

