---
title: แก้ไขปัญหา .PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573903"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="86ac5-102">แก้ไขปัญหา .PRT</span><span class="sxs-lookup"><span data-stu-id="86ac5-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="86ac5-103">สำหรับอุปกรณ์ใดก็ตามที่ต้องการรับการรับรองความถูกต้องจะต้องมีการลงทะเบียนทั้งหมดและในสถานะที่ดีและสามารถรับโทเค็นการรีเฟรชหลัก (.PRT) ได้</span><span class="sxs-lookup"><span data-stu-id="86ac5-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="86ac5-104">กระบวนการลงทะเบียนการเข้าร่วม AD Azure แบบไฮบริดจำเป็นต้องมีอุปกรณ์ที่จะอยู่บนเครือข่ายขององค์กร</span><span class="sxs-lookup"><span data-stu-id="86ac5-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="86ac5-105">นอกจากนี้ยังทำงานผ่าน VPN แต่มีเตือนบางอย่างที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="86ac5-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="86ac5-106">เราเคยได้ยินลูกค้าจำเป็นต้องมีความช่วยเหลือเกี่ยวกับการแก้ไขปัญหาการลงทะเบียนการเข้าร่วม AD Azure ของไฮบริดภายใต้สถานการณ์การทำงานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="86ac5-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="86ac5-107">ต่อไปนี้เป็นรายละเอียดของสิ่งที่เกิดขึ้น ' ภายใต้เครื่องดูดควัน ' ในระหว่างขั้นตอนการลงทะเบียน</span><span class="sxs-lookup"><span data-stu-id="86ac5-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="86ac5-108">**สภาพแวดล้อมการรับรองความถูกต้องของระบบคลาวด์ (โดยใช้การซิงค์แฮชของรหัสผ่าน Azure AD หรือการรับรองความถูกต้องแบบพาส**</span><span class="sxs-lookup"><span data-stu-id="86ac5-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="86ac5-109">ขั้นตอนการลงทะเบียนนี้เรียกว่า "การเข้าร่วมการซิงค์"</span><span class="sxs-lookup"><span data-stu-id="86ac5-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="86ac5-110">Windows 10 จะค้นพบระเบียน SCP เมื่อผู้ใช้เข้าสู่ระบบไปยังอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="86ac5-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="86ac5-111">อุปกรณ์แรกพยายามเรียกข้อมูลผู้เช่าจาก SCP ฝั่งไคลเอ็นต์ในรีจิสทรี [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]</span><span class="sxs-lookup"><span data-stu-id="86ac5-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="86ac5-112">สำหรับข้อมูลเพิ่มเติมให้ดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)นี้</span><span class="sxs-lookup"><span data-stu-id="86ac5-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="86ac5-113">ถ้าล้มเหลวอุปกรณ์จะสื่อสารกับ Active directory ภายในองค์กร (AD) เพื่อรับข้อมูลผู้เช่าจากจุดเชื่อมต่อบริการ (SCP)</span><span class="sxs-lookup"><span data-stu-id="86ac5-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="86ac5-114">เมื่อต้องการตรวจสอบ SCP โปรดดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)นี้</span><span class="sxs-lookup"><span data-stu-id="86ac5-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="86ac5-115">เราขอแนะนำให้ทำการเปิดใช้งาน SCP ในโฆษณาและใช้การตรวจสอบความถูกต้องของการเริ่มต้นที่ด้านไคลเอ็นต์</span><span class="sxs-lookup"><span data-stu-id="86ac5-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="86ac5-116">Windows 10 พยายามสื่อสารกับ Azure AD ภายใต้บริบทของระบบเพื่อรับรองความถูกต้องของตัวเองจาก Azure AD</span><span class="sxs-lookup"><span data-stu-id="86ac5-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="86ac5-117">คุณสามารถตรวจสอบว่าอุปกรณ์สามารถเข้าถึงทรัพยากรของ Microsoft ภายใต้บัญชีผู้ใช้ของระบบโดยใช้สคริปต์การเชื่อมต่อการลงทะเบียนอุปกรณ์ทดสอบ</span><span class="sxs-lookup"><span data-stu-id="86ac5-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="86ac5-118">Windows 10 จะสร้างใบรับรองที่เซ็นชื่อด้วยตนเองและจัดเก็บไว้ภายใต้วัตถุคอมพิวเตอร์ในโฆษณาภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="86ac5-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="86ac5-119">สิ่งนี้จำเป็นต้องใช้ตัวควบคุมโดเมนในสาย</span><span class="sxs-lookup"><span data-stu-id="86ac5-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="86ac5-120">วัตถุอุปกรณ์ที่มีใบรับรองจะได้รับการซิงโครไนซ์กับ Azure AD ผ่าน Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="86ac5-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="86ac5-121">การซิงค์วงจรคือทุกๆ30นาทีตามค่าเริ่มต้นแต่จะขึ้นอยู่กับการกำหนดค่าของ Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="86ac5-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="86ac5-122">สำหรับข้อมูลเพิ่มเติมโปรดดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)นี้</span><span class="sxs-lookup"><span data-stu-id="86ac5-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="86ac5-123">ในขั้นตอนนี้คุณควรจะสามารถเห็นอุปกรณ์เรื่องในสถานะ "ค้างอยู่" ภายใต้ใบพัดของอุปกรณ์ของ Azure Portal</span><span class="sxs-lookup"><span data-stu-id="86ac5-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="86ac5-124">ที่ผู้ใช้ถัดไปเข้าสู่ระบบ Windows 10 การลงทะเบียนจะเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="86ac5-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="86ac5-125">ถ้าคุณอยู่ใน VPN และกระบวนการออกจากระบบ-การเข้าสู่ระบบจะสิ้นสุดลงการเชื่อมต่อโดเมนคุณสามารถทริกเกอร์การลงทะเบียนด้วยตนเองได้:</span><span class="sxs-lookup"><span data-stu-id="86ac5-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="86ac5-126">ออกจาก dsregcmd/join ภายในเครื่องบนพร้อมท์ของผู้ดูแลระบบหรือจากระยะไกลผ่าน PSExec ไปยังพีซีของคุณ</span><span class="sxs-lookup"><span data-stu-id="86ac5-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="86ac5-127">ตัวอย่างเช่น PsExec-s \\ win10client01 cmd, dsregcmd/join</span><span class="sxs-lookup"><span data-stu-id="86ac5-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="86ac5-128">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาการรวมแบบไฮบริดให้ดูที่[แก้ไขปัญหาเกี่ยวกับอุปกรณ์](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)</span><span class="sxs-lookup"><span data-stu-id="86ac5-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
