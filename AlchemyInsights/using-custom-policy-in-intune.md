---
title: ใช้โปรไฟล์แบบกําหนดเองใน Intune
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
- "1566"
- "6700005"
ms.openlocfilehash: 9c7908ef11a26fd83ca83e8c134708687f6d750f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710498"
---
# <a name="using-custom-policy-in-intune"></a><span data-ttu-id="d2ac6-102">การใช้นโยบายแบบกําหนดเองใน Intune</span><span class="sxs-lookup"><span data-stu-id="d2ac6-102">Using custom policy in Intune</span></span>

<span data-ttu-id="d2ac6-103">Intune มีการตั้งค่ามากมายในตัวสําหรับอุปกรณ์ Android, iOS, macOS และ Windows</span><span class="sxs-lookup"><span data-stu-id="d2ac6-103">Intune has many settings built-in for Android, iOS, macOS and Windows devices.</span></span> <span data-ttu-id="d2ac6-104">คุณยังสามารถสร้างโปรไฟล์แบบกําหนดเอง แล้วปรับใช้การตั้งค่าแบบกําหนดเองเหล่านี้ไปยังอุปกรณ์ของคุณโดยใช้ Intune</span><span class="sxs-lookup"><span data-stu-id="d2ac6-104">You can also create a custom profile, and then deploy these custom settings to your devices using Intune.</span></span> <span data-ttu-id="d2ac6-105">โปรไฟล์ที่กําหนดเองได้รับการออกแบบมาเพื่อเพิ่มการตั้งค่าอุปกรณ์และคุณลักษณะที่ไม่ได้สร้างขึ้นใน Intune</span><span class="sxs-lookup"><span data-stu-id="d2ac6-105">Custom profiles are designed to add device settings and features that aren't built in to Intune.</span></span>

[<span data-ttu-id="d2ac6-106">การตั้งค่าแบบกําหนดเองสําหรับอุปกรณ์ Android ใน Intune</span><span class="sxs-lookup"><span data-stu-id="d2ac6-106">Custom settings for Android devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-android)

[<span data-ttu-id="d2ac6-107">การตั้งค่าแบบกําหนดเองสําหรับอุปกรณ์ Android องค์กรใน Intune</span><span class="sxs-lookup"><span data-stu-id="d2ac6-107">Custom settings for Android Enterprise devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-android-for-work)

[<span data-ttu-id="d2ac6-108">การตั้งค่าแบบกําหนดเองสําหรับอุปกรณ์ iOS ใน Intune</span><span class="sxs-lookup"><span data-stu-id="d2ac6-108">Custom settings for iOS devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-ios)

[<span data-ttu-id="d2ac6-109">การตั้งค่าแบบกําหนดเองสําหรับอุปกรณ์ macOS ใน Intune</span><span class="sxs-lookup"><span data-stu-id="d2ac6-109">Custom settings for macOS devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-macos)

[<span data-ttu-id="d2ac6-110">การตั้งค่าแบบกําหนดเองสําหรับอุปกรณ์ Windows 10 ใน Intune</span><span class="sxs-lookup"><span data-stu-id="d2ac6-110">Custom settings for Windows 10 devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-windows-10)

[<span data-ttu-id="d2ac6-111">การตั้งค่าแบบกําหนดเองสําหรับ Windows โฮโลแกรมสําหรับอุปกรณ์ทางธุรกิจใน Intune</span><span class="sxs-lookup"><span data-stu-id="d2ac6-111">Custom settings for Windows Holographic for Business devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-windows-holographic)