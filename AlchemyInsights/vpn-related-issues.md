---
title: ปัญหาที่เกี่ยวข้องกับ VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726110"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="0adf9-102">ปัญหาที่เกี่ยวข้องกับ VPN</span><span class="sxs-lookup"><span data-stu-id="0adf9-102">VPN related issues</span></span>

<span data-ttu-id="0adf9-103">การดำเนินการที่ประสบความสำเร็จของการเชื่อมต่อ VPN สำหรับไคลเอ็นต์ MDM ขึ้นอยู่กับโปรไฟล์ที่ปรับใช้ซึ่งแสดงความต้องการของโครงสร้างพื้นฐานของ VPN อย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="0adf9-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="0adf9-104">สำหรับการตั้งค่าที่เหมาะสมสำหรับแพลตฟอร์มไคลเอ็นต์ที่คุณกำลังตรวจสอบให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="0adf9-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="0adf9-105">การตั้งค่าอุปกรณ์ windows 10 และ Windows ที่ใช้งานโฮโลแกรมเพื่อเพิ่มการเชื่อมต่อ VPN โดยใช้ Intune</span><span class="sxs-lookup"><span data-stu-id="0adf9-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="0adf9-106">เพิ่มการตั้งค่า VPN บนอุปกรณ์ iOS และ iPadOS ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0adf9-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="0adf9-107">การตั้งค่าอุปกรณ์ Android เพื่อกำหนดค่า VPN ใน Intune</span><span class="sxs-lookup"><span data-stu-id="0adf9-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="0adf9-108">เพิ่มการตั้งค่า VPN บนอุปกรณ์ macOS ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0adf9-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="0adf9-109">ถ้าโปรไฟล์ VPN ของคุณใช้การรับรองความถูกต้องโดยใช้ใบรับรองตรวจสอบให้แน่ใจว่าโปรไฟล์ใบรับรองหลักและใบรับรองการรับรองความถูกต้องของไคลเอ็นต์ที่ลิงก์ไปยังโปรไฟล์ VPN ถูกปรับใช้เสร็จเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="0adf9-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="0adf9-110">**ปัญหาทั่วไป**</span><span class="sxs-lookup"><span data-stu-id="0adf9-110">**Common Issues**</span></span>

<span data-ttu-id="0adf9-111">**ฉันจัดวางโปรไฟล์ VPN ไปยังอุปกรณ์ Intune จะแสดงว่าเสร็จเรียบร้อยแล้วแต่อุปกรณ์ไม่ได้เชื่อมต่อกับ VPN**</span><span class="sxs-lookup"><span data-stu-id="0adf9-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="0adf9-112">สถานะที่เสร็จสมบูรณ์หมายความว่า Intune ได้ปรับใช้โปรไฟล์ตามที่ได้รับการกำหนดค่าเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="0adf9-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="0adf9-113">อย่างไรก็ตามการกำหนดค่าเหล่านี้อาจไม่ตรงกับความต้องการของเครือข่ายและ/หรือการรับรองความถูกต้องของคุณ</span><span class="sxs-lookup"><span data-stu-id="0adf9-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="0adf9-114">ตรวจทานบันทึกในบริการโครงสร้างพื้นฐานและการรับรองความถูกต้อง (บนเซิร์ฟเวอร์ VPN และเซิร์ฟเวอร์ NPS/Radius) สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับการเชื่อมต่อที่พยายาม</span><span class="sxs-lookup"><span data-stu-id="0adf9-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="0adf9-115">คุณอาจจำเป็นต้องทำงานกับทีมโครงสร้างพื้นฐานของเครือข่ายของคุณหรือผู้จำหน่าย VPN ของบริษัทอื่นเพื่อรวบรวมและตรวจทานบันทึก</span><span class="sxs-lookup"><span data-stu-id="0adf9-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="0adf9-116">**เมื่อฉันกำหนดค่า VPN แบบกำหนดเองสำหรับ iOS ฟีเจอร์ VPN สำหรับแต่ละแอปจะไม่พร้อมใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="0adf9-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="0adf9-117">สำหรับอุปกรณ์ iOS สำหรับอุปกรณ์ iOS ใน Intune จะพร้อมใช้งานสำหรับรายการของผู้ให้บริการและคู่ค้าที่เฉพาะเจาะจงซึ่งจะต้องตรงตามข้อกำหนดเบื้องต้นของใบรับรองก่อนที่จะกำหนดค่า VPN สำหรับแต่ละแอป</span><span class="sxs-lookup"><span data-stu-id="0adf9-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="0adf9-118">สำหรับข้อมูลเพิ่มเติมให้ดูที่[ตั้งค่าเครือข่ายส่วนตัวเสมือนสำหรับแอป (VPN) สำหรับอุปกรณ์ iOS/iPadOS ใน Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)</span><span class="sxs-lookup"><span data-stu-id="0adf9-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="0adf9-119">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับชนิดการเชื่อมต่อ VPN ทั้งหมดใน Intune ให้ดู[ที่สร้างโปรไฟล์ vpn เพื่อเชื่อมต่อกับเซิร์ฟเวอร์ vpn ใน Intune](https://docs.microsoft.com/intune/vpn-settings-configure)</span><span class="sxs-lookup"><span data-stu-id="0adf9-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="0adf9-120">**VPN ตามความต้องการของ iOS จะไม่ถูกเรียกเมื่อมีการเข้าถึงโดเมนที่กำหนดค่าไว้**</span><span class="sxs-lookup"><span data-stu-id="0adf9-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="0adf9-121">เมื่อต้องการทดสอบการตั้งค่า VPN อัตโนมัติให้ตั้งค่าต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0adf9-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="0adf9-122">ฉันต้องการดำเนินการดังต่อไปนี้: **ประเมินความพยายามในการเชื่อมต่อแต่ละรายการ**</span><span class="sxs-lookup"><span data-stu-id="0adf9-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="0adf9-123">เลือกว่าจะเชื่อมต่อหรือไม่: **เชื่อมต่อถ้าจำเป็น**</span><span class="sxs-lookup"><span data-stu-id="0adf9-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="0adf9-124">เมื่อผู้ใช้เข้าถึงโดเมนเหล่านี้:*ชื่อโดเมน\*\*\*เป้าหมาย*\*</span><span class="sxs-lookup"><span data-stu-id="0adf9-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="0adf9-125">ถ้าการกำหนดค่าด้านบนไม่สำเร็จให้เพิ่มองค์ประกอบต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0adf9-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="0adf9-126">เมื่อ URL นี้ไม่สามารถเข้าถึงให้บังคับเชื่อมต่อ VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="0adf9-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>