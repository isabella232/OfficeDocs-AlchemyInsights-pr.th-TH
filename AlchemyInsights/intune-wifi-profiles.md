---
title: โปรไฟล์ของ Intune สำหรับ wi-fi
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
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696280"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="01b28-102">โปรไฟล์ของ Intune สำหรับ wi-fi</span><span class="sxs-lookup"><span data-stu-id="01b28-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="01b28-103">การดำเนินการการเชื่อมต่อ Wi-fi ที่ประสบความสำเร็จสำหรับไคลเอ็นต์ MDM จะขึ้นอยู่กับโปรไฟล์ที่มีการปรับใช้อย่างถูกต้องซึ่งแสดงถึงความต้องการของโครงสร้างพื้นฐาน Wi-fi ขององค์กร</span><span class="sxs-lookup"><span data-stu-id="01b28-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="01b28-104">เมื่อต้องการตรวจสอบการตั้งค่าที่เหมาะสมสำหรับแพลตฟอร์มไคลเอ็นต์ที่คุณกำลังตรวจสอบให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="01b28-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="01b28-105">เพิ่มการตั้งค่า Wi-fi สำหรับอุปกรณ์ที่ใช้ Android ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="01b28-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="01b28-106">เพิ่มการตั้งค่า Wi-fi สำหรับอุปกรณ์ Android ที่เฉพาะเจาะจงและมีการจัดการทั้งหมดใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="01b28-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="01b28-107">เพิ่มการตั้งค่า Wi-fi สำหรับอุปกรณ์ iOS และ iPadOS ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="01b28-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="01b28-108">เพิ่มการตั้งค่า Wi-fi สำหรับ Windows 10 และอุปกรณ์รุ่นที่ใหม่กว่าใน Intune</span><span class="sxs-lookup"><span data-stu-id="01b28-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="01b28-109">นำเข้าการตั้งค่า wi-fi สำหรับอุปกรณ์ Windows ใน Intune</span><span class="sxs-lookup"><span data-stu-id="01b28-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="01b28-110">**ปัญหาทั่วไป**</span><span class="sxs-lookup"><span data-stu-id="01b28-110">**Common Issues**</span></span>

<span data-ttu-id="01b28-111">**ฉันกำลังปรับใช้โปรไฟล์ Wi-fi ที่ขึ้นอยู่กับใบรับรองที่มีการปรับใช้ที่ระบุไว้ในโปรไฟล์ Wi-Fi อย่างไรก็ตามโปรไฟล์การกำหนดค่าจะแสดงสถานะข้อผิดพลาด**</span><span class="sxs-lookup"><span data-stu-id="01b28-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="01b28-112">ตรวจสอบว่าอุปกรณ์ของคุณได้รับใบรับรองแล้วหรือไม่</span><span class="sxs-lookup"><span data-stu-id="01b28-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="01b28-113">ใน Intune ให้ไปที่**อุปกรณ์ทั้งหมด**แล้วเลือกอุปกรณ์ >**การกำหนดค่าอุปกรณ์**</span><span class="sxs-lookup"><span data-stu-id="01b28-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="01b28-114">ตรวจสอบว่าโปรไฟล์ที่คาดไว้ทั้งหมดอยู่ในรายการและสถานะที่เสร็จสมบูรณ์แล้ว</span><span class="sxs-lookup"><span data-stu-id="01b28-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="01b28-115">สำหรับโปรไฟล์ Android ถ้าคุณมีใบรับรองระดับกลางในสายใบรับรองของคุณให้ตรวจสอบให้แน่ใจว่าพวกเขาได้รับการปรับใช้กับอุปกรณ์ Android</span><span class="sxs-lookup"><span data-stu-id="01b28-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="01b28-116">เมื่อต้องการตรวจสอบสถานะใบรับรองให้ไปที่โปรไฟล์**การกำหนดค่าอุปกรณ์**  >  **Profiles**  >  **Android คุณสมบัติ CA กลาง**  >  **Properties**  >  ที่**เชื่อถือได้ใบรับรองที่เชื่อถือ**ได้</span><span class="sxs-lookup"><span data-stu-id="01b28-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="01b28-117">ถ้าคุณยังคงเห็นข้อผิดพลาดให้ตรวจทานขั้นตอนและการแก้ไขปัญหาส่วน</span><span class="sxs-lookup"><span data-stu-id="01b28-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="01b28-118">สำหรับข้อมูลเพิ่มเติมให้ดูที่[ภาพรวมสำหรับการแก้ไขปัญหาส่วนกำหนดค่า SCEP ที่มี Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="01b28-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="01b28-119">**ฉันจัดวางโปรไฟล์ Wi-fi ไปยังอุปกรณ์ Intune จะแสดงว่าเสร็จเรียบร้อยแล้วแต่อุปกรณ์ไม่ได้เชื่อมต่อกับ Wi-fi**</span><span class="sxs-lookup"><span data-stu-id="01b28-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="01b28-120">สถานะที่เสร็จสมบูรณ์หมายความว่า Intune ได้ปรับใช้โปรไฟล์ตามที่ได้รับการกำหนดค่าเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="01b28-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="01b28-121">อย่างไรก็ตามการกำหนดค่าเหล่านี้อาจไม่ตรงกับความต้องการของเครือข่ายและ/หรือการรับรองความถูกต้องของคุณ</span><span class="sxs-lookup"><span data-stu-id="01b28-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="01b28-122">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับการเชื่อมต่อที่พยายามตรวจสอบบันทึกในบริการโครงสร้างพื้นฐานและการรับรองความถูกต้อง (บนเซิร์ฟเวอร์ตัวควบคุมจุดเข้าใช้งาน Wi-fi และ NPS/Radius)</span><span class="sxs-lookup"><span data-stu-id="01b28-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="01b28-123">คุณอาจต้องทำงานกับทีมโครงสร้างพื้นฐานเครือข่ายของคุณหรือผู้จำหน่าย wi-fi ของบริษัทอื่นเพื่อรวบรวมและตรวจทานบันทึก</span><span class="sxs-lookup"><span data-stu-id="01b28-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>