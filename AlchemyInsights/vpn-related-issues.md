---
title: ปัญหาที่เกี่ยวข้องกับ VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555743"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="9ed7c-102">ปัญหาที่เกี่ยวข้องกับ VPN</span><span class="sxs-lookup"><span data-stu-id="9ed7c-102">VPN related issues</span></span>

<span data-ttu-id="9ed7c-103">การดําเนินการที่ประสบความสําเร็จของการเชื่อมต่อ VPN สําหรับไคลเอนต์ MDM ขึ้นอยู่กับโปรไฟล์ที่ปรับใช้ที่สะท้อนถึงความต้องการของโครงสร้างพื้นฐาน VPN ได้อย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="9ed7c-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="9ed7c-104">สําหรับการตั้งค่าที่เหมาะสมสําหรับแพลตฟอร์มไคลเอ็นต์ที่คุณกําลังตรวจสอบ โปรดดู:</span><span class="sxs-lookup"><span data-stu-id="9ed7c-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="9ed7c-105">การตั้งค่าอุปกรณ์ Windows 10 และ Windows โฮโลแกรมเพื่อเพิ่มการเชื่อมต่อ VPN โดยใช้ Intun</span><span class="sxs-lookup"><span data-stu-id="9ed7c-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="9ed7c-106">เพิ่มการตั้งค่า VPN บนอุปกรณ์ iOS และ iPadOS ใน Microsoft Intuni</span><span class="sxs-lookup"><span data-stu-id="9ed7c-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="9ed7c-107">การตั้งค่าอุปกรณ์ Android เพื่อกําหนดค่า VPN ใน Intun</span><span class="sxs-lookup"><span data-stu-id="9ed7c-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="9ed7c-108">เพิ่มการตั้งค่า VPN บนอุปกรณ์ macOS ใน Microsoft Intun</span><span class="sxs-lookup"><span data-stu-id="9ed7c-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="9ed7c-109">ถ้าส่วนกําหนดค่า VPN ของคุณใช้ใบรับรองการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="9ed7c-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="9ed7c-110">**ปัญหาทั่วไป**</span><span class="sxs-lookup"><span data-stu-id="9ed7c-110">**Common Issues**</span></span>

<span data-ttu-id="9ed7c-111">**ฉันปรับใช้โปรไฟล์ VPN ไปยังอุปกรณ์ Intunเป็นแสดงให้เห็นว่ามันประสบความสําเร็จ, แต่อุปกรณ์ไม่ได้เชื่อมต่อกับ VPN.**</span><span class="sxs-lookup"><span data-stu-id="9ed7c-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="9ed7c-112">สถานะสําเร็จหมายความว่า Intuna ได้ปรับใช้ส่วนกําหนดค่าเป็นการกําหนดค่าเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="9ed7c-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="9ed7c-113">อย่างไรก็ตาม การกําหนดค่าเหล่านี้อาจไม่ตรงกับข้อกําหนดของเครือข่ายและ/หรือการรับรองความถูกต้องของคุณ</span><span class="sxs-lookup"><span data-stu-id="9ed7c-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="9ed7c-114">ตรวจสอบบันทึกในโครงสร้างพื้นฐานและบริการการรับรองความถูกต้อง (บนเซิร์ฟเวอร์ VPN และเซิร์ฟเวอร์ NPS/Radius) สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับการเชื่อมต่อที่พยายาม</span><span class="sxs-lookup"><span data-stu-id="9ed7c-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="9ed7c-115">คุณอาจต้องทํางานร่วมกับทีมโครงสร้างพื้นฐานเครือข่ายของคุณ หรือผู้จําหน่าย VPN ของบริษัทอื่น เพื่อรวบรวมและตรวจสอบบันทึก</span><span class="sxs-lookup"><span data-stu-id="9ed7c-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="9ed7c-116">**เมื่อฉันกําหนดค่า VPN แบบกําหนดเองสําหรับ iOS ฟีเจอร์ VPN ต่อแอปไม่พร้อมใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="9ed7c-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="9ed7c-117">ขณะนี้ VPN ต่อแอปสําหรับอุปกรณ์ iOS ใน Intun ณีมีให้บริการในรายการผู้ให้บริการและคู่ค้าเฉพาะรายซึ่งต้องเป็นไปตามข้อกําหนดเบื้องต้นของใบรับรองก่อนที่จะกําหนดค่า VPN ต่อแอป</span><span class="sxs-lookup"><span data-stu-id="9ed7c-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="9ed7c-118">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ตั้งค่าเครือข่ายส่วนตัวเสมือน (VPN) สําหรับ iOS/iPadOS ใน Intuni](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)</span><span class="sxs-lookup"><span data-stu-id="9ed7c-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="9ed7c-119">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับชนิดการเชื่อมต่อ VPN ทั้งหมดใน Intun [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure)</span><span class="sxs-lookup"><span data-stu-id="9ed7c-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="9ed7c-120">**iOS VPN ตามความต้องการจะไม่ทริกเกอร์เมื่อมีการเข้าถึงโดเมนที่กําหนดค่าไว้**</span><span class="sxs-lookup"><span data-stu-id="9ed7c-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="9ed7c-121">เมื่อต้องการทดสอบการตั้งค่า VPN อัตโนมัติ ให้ตั้งค่าต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="9ed7c-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="9ed7c-122">ฉันต้องการทําดังนี้:**ประเมินความพยายามในการเชื่อมต่อแต่ละครั้ง**</span><span class="sxs-lookup"><span data-stu-id="9ed7c-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="9ed7c-123">เลือกว่าจะเชื่อมต่อหรือไม่:**เชื่อมต่อหากจําเป็น**</span><span class="sxs-lookup"><span data-stu-id="9ed7c-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="9ed7c-124">เมื่อผู้ใช้เข้าถึงโดเมนเหล่านี้:\**ชื่อโดเมนเป้าหมาย\*\*\*domain name*</span><span class="sxs-lookup"><span data-stu-id="9ed7c-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="9ed7c-125">ถ้าการตั้งค่าคอนฟิกข้างต้นไม่สําเร็จ ให้เพิ่มองค์ประกอบต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="9ed7c-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="9ed7c-126">เมื่อ URL นี้ไม่สามารถเข้าถึง บังคับเชื่อมต่อ VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="9ed7c-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>