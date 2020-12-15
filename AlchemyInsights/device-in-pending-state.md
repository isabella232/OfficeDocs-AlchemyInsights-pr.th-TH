---
title: อุปกรณ์ในสถานะที่ค้างอยู่
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679994"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="951ff-102">อุปกรณ์ในสถานะที่ค้างอยู่</span><span class="sxs-lookup"><span data-stu-id="951ff-102">Device in pending state</span></span>

<span data-ttu-id="951ff-103">**เบื้อง**</span><span class="sxs-lookup"><span data-stu-id="951ff-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="951ff-104">ถ้าคุณกำลังตั้งค่าการลงทะเบียนอุปกรณ์เป็นครั้งแรกโปรดตรวจสอบให้แน่ใจว่าคุณได้ตรวจทาน [บทนำสู่การจัดการอุปกรณ์ใน Azure active directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) ที่จะแนะนำคุณเกี่ยวกับวิธีการรับอุปกรณ์ภายใต้การควบคุมของ azure AD</span><span class="sxs-lookup"><span data-stu-id="951ff-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="951ff-105">ถ้าคุณกำลังลงทะเบียนอุปกรณ์ลงใน Azure AD โดยตรงและการลงชื่อเข้าใช้ใน Intune คุณจำเป็นต้องตรวจสอบให้แน่ใจว่าคุณได้ [กำหนดค่า intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) และให้ [สิทธิ์](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) การใช้งานเป็นอันดับแรก</span><span class="sxs-lookup"><span data-stu-id="951ff-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="951ff-106">ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดำเนินการในโฆษณา Azure และโฆษณาภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="951ff-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="951ff-107">เฉพาะผู้ดูแลระบบส่วนกลางใน Azure AD เท่านั้นที่สามารถจัดการการตั้งค่าสำหรับการลงทะเบียนอุปกรณ์ได้</span><span class="sxs-lookup"><span data-stu-id="951ff-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="951ff-108">นอกจากนี้ถ้าคุณกำลังตั้งค่าการลงทะเบียนอัตโนมัติใน active directory ภายในองค์กรของคุณคุณจะต้องเป็นผู้ดูแลไดเรกทอรีที่ใช้งานอยู่และ FS โฆษณา (ถ้ามี)</span><span class="sxs-lookup"><span data-stu-id="951ff-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="951ff-109">กระบวนการลงทะเบียนการเข้าร่วม AD Azure แบบไฮบริดจำเป็นต้องมีอุปกรณ์ที่จะอยู่บนเครือข่ายขององค์กร</span><span class="sxs-lookup"><span data-stu-id="951ff-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="951ff-110">นอกจากนี้ยังทำงานผ่าน VPN แต่มีเตือนบางอย่างที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="951ff-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="951ff-111">เราได้ยินลูกค้าที่จำเป็นต้องมีความช่วยเหลือเกี่ยวกับการแก้ไขปัญหาการลงทะเบียนการเข้าร่วม AD Azure ของไฮบริดภายใต้สถานการณ์การทำงานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="951ff-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="951ff-112">**สภาพแวดล้อมการรับรองความถูกต้องของระบบคลาวด์ (โดยใช้การซิงค์แฮชของรหัสผ่าน Azure AD หรือการรับรองความถูกต้องแบบพาส**</span><span class="sxs-lookup"><span data-stu-id="951ff-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="951ff-113">ขั้นตอนการลงทะเบียนนี้เรียกว่า "การเข้าร่วมการซิงค์"</span><span class="sxs-lookup"><span data-stu-id="951ff-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="951ff-114">ต่อไปนี้เป็นรายละเอียดของสิ่งที่เกิดขึ้นระหว่างขั้นตอนการลงทะเบียน:</span><span class="sxs-lookup"><span data-stu-id="951ff-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="951ff-115">Windows 10 จะค้นพบระเบียนจุดเชื่อมต่อบริการ (SCP) เมื่อผู้ใช้เข้าสู่ระบบอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="951ff-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="951ff-116">อุปกรณ์แรกพยายามเรียกข้อมูลผู้เช่าจาก SCP ฝั่งไคลเอ็นต์ในรีจิสทรี [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]</span><span class="sxs-lookup"><span data-stu-id="951ff-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="951ff-117">สำหรับข้อมูลเพิ่มเติมให้ดูที่[เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)</span><span class="sxs-lookup"><span data-stu-id="951ff-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="951ff-118">ถ้าล้มเหลวอุปกรณ์จะสื่อสารกับไดเรกทอรีที่ใช้งานอยู่ภายในองค์กรเพื่อรับข้อมูลผู้เช่าจาก SCP</span><span class="sxs-lookup"><span data-stu-id="951ff-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="951ff-119">เมื่อต้องการตรวจสอบ SCP ให้ดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)นี้</span><span class="sxs-lookup"><span data-stu-id="951ff-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="951ff-120">เราขอแนะนำให้เปิดใช้งาน SCP ในไดเรกทอรีที่ใช้งานอยู่และใช้ SCP ฝั่งไคลเอ็นต์สำหรับการตรวจสอบความถูกต้องเริ่มต้นเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="951ff-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="951ff-121">Windows 10 พยายามสื่อสารกับ Azure AD ภายใต้บริบทของระบบเพื่อรับรองความถูกต้องของตัวเองจาก Azure AD</span><span class="sxs-lookup"><span data-stu-id="951ff-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="951ff-122">คุณสามารถตรวจสอบว่าอุปกรณ์สามารถเข้าถึงทรัพยากรของ Microsoft ภายใต้บัญชีผู้ใช้ของระบบโดยใช้[สคริปต์การเชื่อมต่อการลงทะเบียนอุปกรณ์ทดสอบ](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)</span><span class="sxs-lookup"><span data-stu-id="951ff-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="951ff-123">Windows 10 จะสร้างใบรับรองที่เซ็นชื่อด้วยตนเองและจัดเก็บไว้ภายใต้วัตถุคอมพิวเตอร์ในไดเรกทอรีที่ใช้งานอยู่ภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="951ff-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="951ff-124">สิ่งนี้จำเป็นต้องใช้ตัวควบคุมโดเมนในสาย</span><span class="sxs-lookup"><span data-stu-id="951ff-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="951ff-125">วัตถุอุปกรณ์ที่มีใบรับรองจะได้รับการซิงโครไนซ์กับ Azure AD ผ่าน Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="951ff-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="951ff-126">การซิงค์วงจรคือทุกๆ30นาทีตามค่าเริ่มต้นแต่จะขึ้นอยู่กับการกำหนดค่าของ Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="951ff-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="951ff-127">สำหรับข้อมูลเพิ่มเติมโปรดดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)นี้</span><span class="sxs-lookup"><span data-stu-id="951ff-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="951ff-128">ในขั้นตอนนี้คุณควรจะสามารถเห็นอุปกรณ์เรื่องในสถานะ "**ค้างอยู่**" ภายใต้ใบพัดของอุปกรณ์ของ Azure Portal</span><span class="sxs-lookup"><span data-stu-id="951ff-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="951ff-129">ที่ผู้ใช้ถัดไปเข้าสู่ระบบ Windows 10 การลงทะเบียนจะเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="951ff-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="951ff-130">ถ้าคุณอยู่ใน VPN และออกจากระบบ/การเข้าสู่ระบบจะสิ้นสุดการเชื่อมต่อโดเมนคุณสามารถทริกเกอร์การลงทะเบียนด้วยตนเองได้</span><span class="sxs-lookup"><span data-stu-id="951ff-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="951ff-131">เมื่อต้องการทำสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="951ff-131">To do that:</span></span>
    >
    > <span data-ttu-id="951ff-132">ออกจาก `dsregcmd /join` พร้อมท์ภายในเครื่องของผู้ดูแลระบบหรือจากระยะไกลผ่านทาง PSExec ไปยังพีซีของคุณ</span><span class="sxs-lookup"><span data-stu-id="951ff-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="951ff-133">ตัวอย่างเช่น: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="951ff-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="951ff-134">สำหรับปัญหาทั่วไปเกี่ยวกับการลงทะเบียนอุปกรณ์ของ Azure Active directory ให้ดูที่คำ[ถามที่ถามบ่อยเกี่ยวกับอุปกรณ์](https://docs.microsoft.com/azure/active-directory/devices/faq)</span><span class="sxs-lookup"><span data-stu-id="951ff-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
