---
title: โปรไฟล์ Wi-Fi แบบ Intun
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555816"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="eb533-102">โปรไฟล์ Wi-Fi แบบ Intun</span><span class="sxs-lookup"><span data-stu-id="eb533-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="eb533-103">การดําเนินการที่ประสบความสําเร็จของการเชื่อมต่อ Wi-Fi สําหรับไคลเอนต์ MDM ขึ้นอยู่กับโปรไฟล์ที่ใช้งานอย่างถูกต้องซึ่งสะท้อนถึงความต้องการของโครงสร้างพื้นฐาน Wi-Fi ขององค์กร</span><span class="sxs-lookup"><span data-stu-id="eb533-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="eb533-104">ในการตรวจสอบการตั้งค่าที่เหมาะสมสําหรับแพลตฟอร์มไคลเอ็นต์ที่คุณกําลังตรวจสอบ โปรดดู:</span><span class="sxs-lookup"><span data-stu-id="eb533-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="eb533-105">เพิ่มการตั้งค่า Wi-Fi สําหรับอุปกรณ์ที่ใช้ Android ใน Microsoft Intun</span><span class="sxs-lookup"><span data-stu-id="eb533-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="eb533-106">เพิ่มการตั้งค่า Wi-Fi สําหรับอุปกรณ์ Android องค์กรที่ทุ่มเทและมีการจัดการอย่างเต็มที่ใน Microsoft Intun</span><span class="sxs-lookup"><span data-stu-id="eb533-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="eb533-107">เพิ่มการตั้งค่า Wi-Fi สําหรับอุปกรณ์ iOS และ iPadOS ใน Microsoft Intuni</span><span class="sxs-lookup"><span data-stu-id="eb533-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="eb533-108">เพิ่มการตั้งค่า Wi-Fi สําหรับ Windows 10 และอุปกรณ์ที่ใหม่กว่าใน Intun</span><span class="sxs-lookup"><span data-stu-id="eb533-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="eb533-109">นําเข้าการตั้งค่า Wi-Fi สําหรับอุปกรณ์ Windows ใน Intun</span><span class="sxs-lookup"><span data-stu-id="eb533-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="eb533-110">**ปัญหาทั่วไป**</span><span class="sxs-lookup"><span data-stu-id="eb533-110">**Common Issues**</span></span>

<span data-ttu-id="eb533-111">**ฉันกําลังปรับใช้โพรไฟล์ Wi-Fi ที่ขึ้นอยู่กับใบรับรองที่ปรับใช้ซึ่งระบุไว้ในโปรไฟล์ Wi-Fi อย่างไรก็ตาม โปรไฟล์การตั้งค่าคอนฟิกจะแสดงสถานะข้อผิดพลาด**</span><span class="sxs-lookup"><span data-stu-id="eb533-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="eb533-112">ตรวจสอบว่าอุปกรณ์ของคุณได้รับใบรับรอง</span><span class="sxs-lookup"><span data-stu-id="eb533-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="eb533-113">ใน Intun เยือกไปที่**อุปกรณ์ทั้งหมด**และเลือกอุปกรณ์>**การกําหนดค่าอุปกรณ์**</span><span class="sxs-lookup"><span data-stu-id="eb533-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="eb533-114">ตรวจสอบว่า โพรไฟล์ที่คาดว่าจะทั้งหมดจะแสดงรายการ และ ในสถานะที่ประสบความสําเร็จ</span><span class="sxs-lookup"><span data-stu-id="eb533-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="eb533-115">สําหรับโปรไฟล์ Android หากคุณมีใบรับรองระดับกลางในห่วงโซ่ใบรับรอง ของคุณ ให้ตรวจสอบให้แน่ใจว่าได้ปรับใช้กับอุปกรณ์ Android แล้ว</span><span class="sxs-lookup"><span data-stu-id="eb533-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="eb533-116">เมื่อต้องการตรวจสอบสถานะใบรับรอง ให้ไปที่**ส่วนกําหนดค่าการกําหนดค่าอุปกรณ์**  >  **Profiles**  >  **Android คุณสมบัติ CA ระดับกลาง**  >  **Properties**  >  **ใบรับรองที่เชื่อถือได้**</span><span class="sxs-lookup"><span data-stu-id="eb533-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="eb533-117">ถ้าคุณยังคงเห็นข้อผิดพลาดให้ตรวจสอบขั้นตอนและส่วนการแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="eb533-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="eb533-118">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ภาพรวมสําหรับการแก้ไขปัญหาโพรไฟล์ใบรับรอง SCEP ด้วย Microsoft Intunณี](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="eb533-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="eb533-119">**ฉันปรับใช้โปรไฟล์ Wi-Fi ไปยังอุปกรณ์ Intunเป็นแสดงว่ามันประสบความสําเร็จ, แต่อุปกรณ์ไม่ได้เชื่อมต่อกับ Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="eb533-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="eb533-120">สถานะสําเร็จหมายความว่า Intuna ได้ปรับใช้ส่วนกําหนดค่าเป็นการกําหนดค่าเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="eb533-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="eb533-121">อย่างไรก็ตาม การกําหนดค่าเหล่านี้อาจไม่ตรงกับข้อกําหนดของเครือข่ายและ/หรือการรับรองความถูกต้องของคุณ</span><span class="sxs-lookup"><span data-stu-id="eb533-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="eb533-122">สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับการเชื่อมต่อที่พยายามให้ตรวจสอบบันทึกในโครงสร้างพื้นฐานและบริการการรับรองความถูกต้อง (ในตัวควบคุมจุดเข้าใช้งาน Wi-Fi และเซิร์ฟเวอร์ NPS/Radius)</span><span class="sxs-lookup"><span data-stu-id="eb533-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="eb533-123">คุณอาจต้องทํางานร่วมกับทีมโครงสร้างพื้นฐานเครือข่ายของคุณ หรือผู้ให้บริการ Wi-Fi บุคคลที่สาม เพื่อรวบรวมและตรวจสอบบันทึก</span><span class="sxs-lookup"><span data-stu-id="eb533-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>