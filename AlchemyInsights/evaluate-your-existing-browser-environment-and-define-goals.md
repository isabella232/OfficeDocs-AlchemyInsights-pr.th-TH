---
title: ประเมินสภาพแวดล้อมเบราว์เซอร์ที่มีอยู่ของคุณและกําหนดเป้าหมาย
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
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694819"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a><span data-ttu-id="64aac-102">ประเมินสภาพแวดล้อมเบราว์เซอร์ที่มีอยู่ของคุณและกําหนดเป้าหมาย</span><span class="sxs-lookup"><span data-stu-id="64aac-102">Evaluate your existing browser environment and define goals</span></span>

<span data-ttu-id="64aac-103">การสละเวลาเพื่อเข้าใจสถานะเบราว์เซอร์และการมองเห็นโครงการปัจจุบันของคุณเพื่อให้แน่ใจว่าผู้เกี่ยวข้องของโครงการทั้งหมดจะถูกจัดแนวและอยู่ในเป้าหมายเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="64aac-103">Taking time to understand your current browser state and project vision ensures all project stakeholders are aligned and are working toward the same goal.</span></span> <span data-ttu-id="64aac-104">ให้ปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="64aac-104">Follow these steps:</span></span>

1. <span data-ttu-id="64aac-105">กําหนดสถานะปัจจุบันของคุณ</span><span class="sxs-lookup"><span data-stu-id="64aac-105">Define your current state.</span></span> <span data-ttu-id="64aac-106">พิจารณาสิ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="64aac-106">Consider the following:</span></span>
- <span data-ttu-id="64aac-107">ขณะนี้เบราว์เซอร์ใดที่ปรับใช้ในสภาพแวดล้อมของคุณ</span><span class="sxs-lookup"><span data-stu-id="64aac-107">Which browsers are currently deployed in your environment?</span></span>
- <span data-ttu-id="64aac-108">เบราว์เซอร์ใดที่ถูกตั้งค่าเป็นเบราว์เซอร์เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="64aac-108">Which browser is set as the default browser?</span></span>
- <span data-ttu-id="64aac-109">คุณต้องใช้ Internet Explorer กับแอปบางแอปของคุณหรือไม่</span><span class="sxs-lookup"><span data-stu-id="64aac-109">Do you need to use Internet Explorer for some of your apps?</span></span>
- <span data-ttu-id="64aac-110">คุณใช้รายการไซต์โหมดองค์กรเพื่อกําหนดค่า Internet Explorer ในปัจจุบันหรือไม่</span><span class="sxs-lookup"><span data-stu-id="64aac-110">Do you use an Enterprise Mode Site List to configure Internet Explorer today?</span></span>
- <span data-ttu-id="64aac-111">แพลตฟอร์ม OS ใด เช่น Windows 10 และ macOS สภาพแวดล้อมของคุณสนับสนุนหรือไม่</span><span class="sxs-lookup"><span data-stu-id="64aac-111">Which OS platforms, such as Windows 10 and macOS, does your environment support?</span></span>
- <span data-ttu-id="64aac-112">คุณใช้เครื่องมือการจัดการใดในการจัดการเบราว์เซอร์</span><span class="sxs-lookup"><span data-stu-id="64aac-112">Which management tools do you use for browser management?</span></span>
- <span data-ttu-id="64aac-113">ใครมีหน้าที่รับผิดชอบในการกําหนดค่าและการจัดการเบราว์เซอร์</span><span class="sxs-lookup"><span data-stu-id="64aac-113">Who's responsible for browser configuration and management?</span></span>
- <span data-ttu-id="64aac-114">กระบวนการตรวจสอบความถูกต้องของความเข้ากันได้ของเบราว์เซอร์คืออะไร</span><span class="sxs-lookup"><span data-stu-id="64aac-114">What's the process for validating browser compatibility?</span></span>
2. <span data-ttu-id="64aac-115">กําหนดเป้าหมายเพื่อการปรับใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="64aac-115">Define the goals for your deployment.</span></span> <span data-ttu-id="64aac-116">โปรดระลึกถึงสิ่งต่างๆ ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="64aac-116">Keep the following things in mind:</span></span>
- <span data-ttu-id="64aac-117">คุณต้องการตั้งค่า Microsoft [Edge เป็นเบราว์เซอร์เริ่มต้น](https://docs.microsoft.com/DeployEdge/edge-default-browser)ของคุณหรือไม่</span><span class="sxs-lookup"><span data-stu-id="64aac-117">Do you want to [set Microsoft Edge as your default browser](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span></span>
- <span data-ttu-id="64aac-118">คุณต้องการซ่อนเวอร์ชันดั้งเดิมของ Microsoft Edge หรือคุณต้องการปล่อยให้ [พร้อมใช้งานกับผู้ใช้](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)หรือไม่</span><span class="sxs-lookup"><span data-stu-id="64aac-118">Do you want to hide the legacy version of Microsoft Edge or do you want to [leave it available for users](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span></span>
- <span data-ttu-id="64aac-119">คุณจะกําหนด [ค่า Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)อย่างไร</span><span class="sxs-lookup"><span data-stu-id="64aac-119">How will you [configure Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span></span>
- <span data-ttu-id="64aac-120">ฟีเจอร์ใดที่มีความร้ายแรงในการกําหนดค่าให้เป็นส่วนหนึ่งของการปรับใช้ครั้งแรกของคุณ</span><span class="sxs-lookup"><span data-stu-id="64aac-120">What features are critical to configure as part of your initial deployment?</span></span>
- <span data-ttu-id="64aac-121">กระบวนการในการระบุปัญหาความเข้ากันได้หรือการกําหนดค่าที่ระบุคืออะไร</span><span class="sxs-lookup"><span data-stu-id="64aac-121">What is the process for addressing any identified compatibility or configuration issues?</span></span>
3. <span data-ttu-id="64aac-122">เข้าใจเบื้องต้นของฟีเจอร์ที่คุณอาจต้องการใช้ เช่น</span><span class="sxs-lookup"><span data-stu-id="64aac-122">Understand the prerequisites for features you might want to use, such as:</span></span>
- [<span data-ttu-id="64aac-123">Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="64aac-123">Windows Defender Application Guard</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [<span data-ttu-id="64aac-124">โหมด Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="64aac-124">Internet Explorer mode</span></span>](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [<span data-ttu-id="64aac-125">การรับรองความถูกต้องและการซิงค์</span><span class="sxs-lookup"><span data-stu-id="64aac-125">Authentication and sync</span></span>](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

<span data-ttu-id="64aac-126">หลังจากเสร็จสิ้นขั้นตอนเหล่านี้แล้ว คุณก็พร้อมที่จะเริ่มวางแผนกลยุทธ์การปรับใช้</span><span class="sxs-lookup"><span data-stu-id="64aac-126">After you complete these steps, you're ready to start planning your deployment strategy.</span></span>
