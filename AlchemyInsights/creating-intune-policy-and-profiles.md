---
title: สร้างนโยบายและโปรไฟล์ Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: fac2a9e41449b4eb9b87d21d4cba4f6f5192d9c6
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715415"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="99fd3-102">การสร้างนโยบาย Intune และโปรไฟล์</span><span class="sxs-lookup"><span data-stu-id="99fd3-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="99fd3-103">ใน Intune คุณสามารถสร้างนโยบายและโปรไฟล์ที่กระทําสิ่งที่แตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="99fd3-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="99fd3-104">**โปรไฟล์การลงทะเบียน**: กําหนดค่าอุปกรณ์ของคุณล่วงหน้าตามแพลตฟอร์มเปิดใช้งานความเกี่ยวข้องของผู้ใช้ใช้การตรวจสอบหลายปัจจัยและอื่น ๆ</span><span class="sxs-lookup"><span data-stu-id="99fd3-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="99fd3-105">[การลงทะเบียนอุปกรณ์คืออะไร](https://docs.microsoft.com/intune/device-enrollment)และสร้างโปรไฟล์การลงทะเบียนสําหรับ[Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll)และ[Windows](https://docs.microsoft.com/intune/windows-enrollment-methods)เป็นแหล่งข้อมูลที่ดี</span><span class="sxs-lookup"><span data-stu-id="99fd3-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="99fd3-106">**นโยบายการปฏิบัติตามกฎระเบียบ**: กําหนดกฎและการตั้งค่าที่อุปกรณ์ต้องปฏิบัติตามเพื่อให้เป็นไปตามข้อกําหนด</span><span class="sxs-lookup"><span data-stu-id="99fd3-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="99fd3-107">นอกจากนี้ คุณยังสามารถใช้นโยบายการปฏิบัติตามนโยบายเพื่อตรวจสอบอุปกรณ์ และแจ้งเตือนผู้ใช้ที่ไม่ปฏิบัติตามนโยบาย</span><span class="sxs-lookup"><span data-stu-id="99fd3-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="99fd3-108">เริ่มต้นใช้งาน[นโยบายการปฏิบัติตามข้อกําหนดของอุปกรณ์](https://docs.microsoft.com/intune/device-compliance-get-started)</span><span class="sxs-lookup"><span data-stu-id="99fd3-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="99fd3-109">**นโยบายการเข้าถึงแบบมีเงื่อนไข**: ช่วยรักษาความปลอดภัยให้กับทรัพยากรขององค์กร โดยขึ้นอยู่กับเงื่อนไขที่คุณป้อน</span><span class="sxs-lookup"><span data-stu-id="99fd3-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="99fd3-110">ตัวอย่างเช่น สําหรับอุปกรณ์ที่ไม่เป็นไปตามข้อกําหนด ให้ใช้การเข้าถึงแบบมีเงื่อนไขเพื่อจํากัดการเข้าถึงอีเมลและ SharePoint</span><span class="sxs-lookup"><span data-stu-id="99fd3-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="99fd3-111">[การเข้าถึงแบบมีเงื่อนไข](https://docs.microsoft.com/intune/conditional-access)[และวิธีการทั่วไปในการใช้การเข้าถึงแบบมีเงื่อนไข](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use)คือทรัพยากรที่ดีในการเริ่มต้นใช้งานคืออะไร</span><span class="sxs-lookup"><span data-stu-id="99fd3-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="99fd3-112">**โปรไฟล์การกําหนดค่า**: จัดการคุณสมบัติและการตั้งค่าบนอุปกรณ์ รวมถึงการตั้งค่าอีเมล เพิ่มเครือข่าย WiFi ใช้เทมเพลตในตัว การควบคุมคุณสมบัติอุปกรณ์ iOS และ macOS และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="99fd3-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="99fd3-113">เริ่มต้นใช้งาน[โปรไฟล์การกําหนดค่าอุปกรณ์](https://docs.microsoft.com/intune/device-profiles)</span><span class="sxs-lookup"><span data-stu-id="99fd3-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="99fd3-114">ลิงค์ที่เป็นประโยชน์:</span><span class="sxs-lookup"><span data-stu-id="99fd3-114">Helpful links:</span></span>

- [<span data-ttu-id="99fd3-115">คําถามทั่วไป ปัญหา และวิธีแก้ปัญหาด้วยนโยบายและโปรไฟล์ของอุปกรณ์ใน Intune</span><span class="sxs-lookup"><span data-stu-id="99fd3-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="99fd3-116">การแก้ไขปัญหานโยบายและโปรไฟล์ใน Intune</span><span class="sxs-lookup"><span data-stu-id="99fd3-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
