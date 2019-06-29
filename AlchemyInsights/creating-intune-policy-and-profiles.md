---
title: สร้างนโยบาย Intune และโพรไฟล์
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 05/07/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: 580903fd89dca8a2ecbf635fa2157f31c93b85f4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363780"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="904a5-102">สร้างนโยบาย Intune และโพรไฟล์</span><span class="sxs-lookup"><span data-stu-id="904a5-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="904a5-103">ใน Intune คุณสามารถสร้างนโยบายและโพรไฟล์ที่ทำสิ่งที่แตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="904a5-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="904a5-104">**โพรไฟล์การลงทะเบียน**: กำหนดการตั้งล่วงหน้าของอุปกรณ์ของคุณ โดยแพลตฟอร์ม ความสัมพันธ์ของผู้ใช้ที่เปิดใช้งาน ใช้การรับรองความถูกต้องด้วยหลายปัจจัย และอื่น ๆ</span><span class="sxs-lookup"><span data-stu-id="904a5-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="904a5-105">การ[ลงทะเบียนอุปกรณ์คืออะไร](https://docs.microsoft.com/intune/device-enrollment)และสร้างโพรไฟล์การลงทะเบียนสำหรับ[Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll)และ[หน้าต่าง](https://docs.microsoft.com/intune/windows-enrollment-methods)ดีทรัพยากรที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="904a5-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="904a5-106">**นโยบายการปฏิบัติตามกฎระเบียบ**: กำหนดกฎและค่าที่อุปกรณ์ต้องปฏิบัติตามเพื่อให้เป็นไปตามกฎ</span><span class="sxs-lookup"><span data-stu-id="904a5-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="904a5-107">คุณสามารถใช้นโยบายการปฏิบัติตามกฎระเบียบเพื่อตรวจสอบอุปกรณ์ และแจ้งเตือนผู้ใช้ของความไม่สอดคล้องกัน</span><span class="sxs-lookup"><span data-stu-id="904a5-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="904a5-108">เริ่มต้นใช้งานกับ[อุปกรณ์นโยบายการปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/intune/device-compliance-get-started)</span><span class="sxs-lookup"><span data-stu-id="904a5-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="904a5-109">**นโยบายการเข้าถึงแบบมีเงื่อนไข**: ช่วยรักษาความปลอดภัยขององค์กรทรัพยากร ขึ้นอยู่กับเงื่อนไขที่คุณป้อน</span><span class="sxs-lookup"><span data-stu-id="904a5-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="904a5-110">ตัวอย่างเช่น สำหรับอุปกรณ์ที่ไม่เข้ากันกับ ใช้ access แบบมีเงื่อนไขเพื่อจำกัดการเข้าถึงอีเมลและ SharePoint</span><span class="sxs-lookup"><span data-stu-id="904a5-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="904a5-111">[วิธีทั่วไปในการใช้การเข้าถึงแบบมีเงื่อนไข](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use)และการ[เข้าถึงแบบมีเงื่อนไขคืออะไร](https://docs.microsoft.com/intune/conditional-access)มีทรัพยากรที่ดีในการเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="904a5-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="904a5-112">**โพรไฟล์การตั้งค่าคอนฟิก**: จัดการลักษณะการทำงานและการตั้งค่าบนอุปกรณ์ รวมทั้งการตั้งค่าอีเมล เพิ่มเครือข่าย WiFi ใช้แม่แบบที่มีอยู่ภายใน คุณลักษณะตัวควบคุม iOS และ macOS อุปกรณ์ และอื่น ๆ</span><span class="sxs-lookup"><span data-stu-id="904a5-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="904a5-113">เริ่มต้นใช้งานใน[ส่วนกำหนดค่าการตั้งค่าคอนฟิกอุปกรณ์](https://docs.microsoft.com/intune/device-profiles)</span><span class="sxs-lookup"><span data-stu-id="904a5-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="904a5-114">การเชื่อมโยงที่เป็นประโยชน์:</span><span class="sxs-lookup"><span data-stu-id="904a5-114">Helpful links:</span></span>

- [<span data-ttu-id="904a5-115">ทั่วไปคำถาม ปัญหา และวิธีแก้ปัญหา ด้วยนโยบายอุปกรณ์และโพรไฟล์ใน Intune</span><span class="sxs-lookup"><span data-stu-id="904a5-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="904a5-116">การแก้ไขปัญหานโยบายและโพรไฟล์ใน Intune</span><span class="sxs-lookup"><span data-stu-id="904a5-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
