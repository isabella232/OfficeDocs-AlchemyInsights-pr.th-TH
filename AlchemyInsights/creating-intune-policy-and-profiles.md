---
title: สร้างนโยบายและโปรไฟล์ Intuny
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: af8f1a3dfaccaca52f187f387274d63b22631b2d
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704661"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="6e01a-102">การสร้างนโยบายและโปรไฟล์ Intun1</span><span class="sxs-lookup"><span data-stu-id="6e01a-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="6e01a-103">Intuny คุณสามารถสร้างนโยบายและโปรไฟล์ที่ปฏิบัติสิ่งต่าง ๆ ได้</span><span class="sxs-lookup"><span data-stu-id="6e01a-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="6e01a-104">**โปรไฟล์การลงทะเบียน**: ตั้งค่าอุปกรณ์ของคุณล่วงหน้าตามแพลตฟอร์ม เปิดใช้งานการยืนยันผู้ใช้ ใช้การรับรองความถูกต้องแบบหลายปัจจัย และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="6e01a-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="6e01a-105">[การลงทะเบียนอุปกรณ์คืออะไร](https://docs.microsoft.com/intune/device-enrollment)และสร้างโปรไฟล์การลงทะเบียน for [Android,](https://docs.microsoft.com/intune/android-enroll) [iOS,](https://docs.microsoft.com/intune/ios-enroll) [macOS](https://docs.microsoft.com/intune/macos-enroll)และ [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) เป็นแหล่งข้อมูลที่ดี</span><span class="sxs-lookup"><span data-stu-id="6e01a-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="6e01a-106">**นโยบายการปฏิบัติตาม** นโยบาย : กําหนดกฎและการตั้งค่าที่อุปกรณ์ต้องปฏิบัติตามให้เป็นไปตามข้อกําหนด</span><span class="sxs-lookup"><span data-stu-id="6e01a-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="6e01a-107">คุณยังสามารถใช้นโยบายการปฏิบัติตามนโยบายเพื่อตรวจสอบอุปกรณ์ และแจ้งให้ผู้ใช้ทราบเกี่ยวกับการปฏิบัติตามข้อบังคับ</span><span class="sxs-lookup"><span data-stu-id="6e01a-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="6e01a-108">เริ่มต้นใช้งานนโยบาย[การปฏิบัติตามนโยบายของอุปกรณ์](https://docs.microsoft.com/intune/device-compliance-get-started)</span><span class="sxs-lookup"><span data-stu-id="6e01a-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="6e01a-109">**นโยบายการเข้าถึงตามเงื่อนไข**: ช่วยรักษาความปลอดภัยของแหล่งข้อมูลขององค์กร โดยขึ้นอยู่กับเงื่อนไขที่คุณใส่</span><span class="sxs-lookup"><span data-stu-id="6e01a-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="6e01a-110">ตัวอย่างเช่น ใช้การเข้าถึงตามเงื่อนไขเพื่อจํากัดการเข้าถึงอีเมลและ SharePoint</span><span class="sxs-lookup"><span data-stu-id="6e01a-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="6e01a-111">[การเข้าถึงตามเงื่อนไขและ](https://docs.microsoft.com/intune/conditional-access)[วิธีทั่วไปในการใช้การเข้าถึงตามเงื่อนไข](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use)คือแหล่งข้อมูลที่ดีในการเริ่มต้นใช้งาน</span><span class="sxs-lookup"><span data-stu-id="6e01a-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="6e01a-112">**โปรไฟล์การกําหนด** ค่า : จัดการฟีเจอร์และการตั้งค่าบนอุปกรณ์ รวมถึงการตั้งค่าอีเมล เพิ่มเครือข่าย WiFi ใช้เทมเพลตที่มีอยู่แล้วภายใน ควบคุมฟีเจอร์ของอุปกรณ์ iOS และ macOS และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="6e01a-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="6e01a-113">เริ่มต้นใช้งานโปรไฟล์ [การกําหนดค่า](https://docs.microsoft.com/intune/device-profiles)อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="6e01a-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="6e01a-114">ลิงก์ที่เป็นประโยชน์:</span><span class="sxs-lookup"><span data-stu-id="6e01a-114">Helpful links:</span></span>

- [<span data-ttu-id="6e01a-115">ข้อถาม ปัญหา และการแก้ไขปัญหาทั่วไปเกี่ยวกับนโยบายอุปกรณ์และโปรไฟล์ใน Intuny</span><span class="sxs-lookup"><span data-stu-id="6e01a-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="6e01a-116">แก้ไขปัญหานโยบายและโปรไฟล์ใน Intun1</span><span class="sxs-lookup"><span data-stu-id="6e01a-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)
