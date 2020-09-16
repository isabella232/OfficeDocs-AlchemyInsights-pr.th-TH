---
title: สร้างนโยบายของ Intune และโปรไฟล์ของ Intune
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
ms.openlocfilehash: 9026beac824ebc3849241dbb534c27b00ef1d0eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47746778"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="2964b-102">การสร้างนโยบายและโพรไฟล์ของ Intune</span><span class="sxs-lookup"><span data-stu-id="2964b-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="2964b-103">ใน Intune คุณสามารถสร้างนโยบายและโปรไฟล์ที่ทำสิ่งต่างๆได้</span><span class="sxs-lookup"><span data-stu-id="2964b-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="2964b-104">**โปรไฟล์การลงทะเบียน**: กำหนดการอุปกรณ์ของคุณตาม platform ให้เปิดใช้งานความสัมพันธ์ของผู้ใช้ใช้การรับรองความถูกต้องแบบหลายปัจจัยและอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="2964b-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="2964b-105">การ[ลงทะเบียนอุปกรณ์คืออะไร](https://docs.microsoft.com/intune/device-enrollment)และสร้างโปรไฟล์การลงทะเบียนสำหรับ[Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll)และ[Windows](https://docs.microsoft.com/intune/windows-enrollment-methods)เป็นแหล่งข้อมูลที่ดี</span><span class="sxs-lookup"><span data-stu-id="2964b-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="2964b-106">**นโยบายการปฏิบัติตามกฎระเบียบ**: กำหนดกฎและการตั้งค่าที่อุปกรณ์ต้องเป็นไปตามเพื่อให้สอดคล้องกัน</span><span class="sxs-lookup"><span data-stu-id="2964b-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="2964b-107">นอกจากนี้คุณยังสามารถใช้นโยบายการปฏิบัติตามนโยบายเพื่อตรวจสอบอุปกรณ์และแจ้งให้ผู้ใช้ที่ไม่ปฏิบัติตามข้อบังคับ</span><span class="sxs-lookup"><span data-stu-id="2964b-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="2964b-108">เริ่มต้นใช้งาน[นโยบายการปฏิบัติตามนโยบายของอุปกรณ์](https://docs.microsoft.com/intune/device-compliance-get-started)</span><span class="sxs-lookup"><span data-stu-id="2964b-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="2964b-109">**นโยบายการเข้าถึงตามเงื่อนไข**: ช่วยรักษาความปลอดภัยทรัพยากรขององค์กรทั้งนี้ขึ้นอยู่กับเงื่อนไขที่คุณใส่</span><span class="sxs-lookup"><span data-stu-id="2964b-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="2964b-110">ตัวอย่างเช่นสำหรับอุปกรณ์ที่ไม่สอดคล้องกันให้ใช้การเข้าถึงตามเงื่อนไขเพื่อจำกัดการเข้าถึงอีเมลและ SharePoint</span><span class="sxs-lookup"><span data-stu-id="2964b-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="2964b-111">การ[เข้าถึงเงื่อนไข](https://docs.microsoft.com/intune/conditional-access)และ[วิธีทั่วไปในการใช้การเข้าถึง](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use)แบบมีเงื่อนไขคือทรัพยากรที่ดีในการเริ่มต้นใช้งาน</span><span class="sxs-lookup"><span data-stu-id="2964b-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="2964b-112">**โปรไฟล์การกำหนดค่า**: จัดการฟีเจอร์และการตั้งค่าบนอุปกรณ์รวมถึงการตั้งค่าอีเมลเพิ่มเครือข่าย WiFi ใช้เทมเพลตที่มีอยู่แล้วภายในตัวควบคุมอุปกรณ์ IOS และ macOS และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="2964b-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="2964b-113">เริ่มต้นใช้งานที่[โปรไฟล์การกำหนดค่าอุปกรณ์](https://docs.microsoft.com/intune/device-profiles)</span><span class="sxs-lookup"><span data-stu-id="2964b-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="2964b-114">ลิงก์ที่มีประโยชน์:</span><span class="sxs-lookup"><span data-stu-id="2964b-114">Helpful links:</span></span>

- [<span data-ttu-id="2964b-115">คำถามทั่วไปปัญหาและวิธีแก้ไขปัญหาเกี่ยวกับนโยบายของอุปกรณ์และโปรไฟล์ใน Intune</span><span class="sxs-lookup"><span data-stu-id="2964b-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="2964b-116">การแก้ไขปัญหานโยบายและโปรไฟล์ใน Intune</span><span class="sxs-lookup"><span data-stu-id="2964b-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
