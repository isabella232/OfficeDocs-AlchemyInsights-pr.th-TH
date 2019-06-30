---
title: ใช้ส่วนกำหนดค่าแบบกำหนดเองใน Intune
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
- "1566"
- "6700005"
ms.openlocfilehash: 300e2e90723ec4d46abeda1a4879e0577193ad05
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365940"
---
# <a name="using-custom-policy-in-intune"></a><span data-ttu-id="9ecb4-102">การใช้นโยบายแบบกำหนดเองใน Intune</span><span class="sxs-lookup"><span data-stu-id="9ecb4-102">Using custom policy in Intune</span></span>

<span data-ttu-id="9ecb4-103">Intune มีหลายการตั้งค่าสำหรับอุปกรณ์ Android, iOS, macOS และ Windows</span><span class="sxs-lookup"><span data-stu-id="9ecb4-103">Intune has many settings built-in for Android, iOS, macOS and Windows devices.</span></span> <span data-ttu-id="9ecb4-104">คุณสามารถสร้างส่วนกำหนดค่าแบบกำหนดเอง และจากนั้น ปรับใช้การตั้งค่าแบบกำหนดเองเหล่านี้ไปยังอุปกรณ์ของคุณโดยใช้ Intune</span><span class="sxs-lookup"><span data-stu-id="9ecb4-104">You can also create a custom profile, and then deploy these custom settings to your devices using Intune.</span></span> <span data-ttu-id="9ecb4-105">ส่วนกำหนดค่าแบบกำหนดเองถูกออกแบบมาเพื่อเพิ่มการตั้งค่าอุปกรณ์และคุณลักษณะที่ไม่ได้อยู่ภายใน Intune</span><span class="sxs-lookup"><span data-stu-id="9ecb4-105">Custom profiles are designed to add device settings and features that aren't built in to Intune.</span></span>

[<span data-ttu-id="9ecb4-106">การตั้งค่าแบบกำหนดเองสำหรับอุปกรณ์ Android ใน Intune</span><span class="sxs-lookup"><span data-stu-id="9ecb4-106">Custom settings for Android devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-android)

[<span data-ttu-id="9ecb4-107">การตั้งค่าแบบกำหนดเองสำหรับอุปกรณ์ Android องค์กรใน Intune</span><span class="sxs-lookup"><span data-stu-id="9ecb4-107">Custom settings for Android Enterprise devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-android-for-work)

[<span data-ttu-id="9ecb4-108">การตั้งค่าแบบกำหนดเองสำหรับอุปกรณ์ iOS ใน Intune</span><span class="sxs-lookup"><span data-stu-id="9ecb4-108">Custom settings for iOS devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-ios)

[<span data-ttu-id="9ecb4-109">การตั้งค่าแบบกำหนดเองสำหรับอุปกรณ์ macOS ใน Intune</span><span class="sxs-lookup"><span data-stu-id="9ecb4-109">Custom settings for macOS devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-macos)

[<span data-ttu-id="9ecb4-110">การตั้งค่าแบบกำหนดเองสำหรับอุปกรณ์ Windows 10 ใน Intune</span><span class="sxs-lookup"><span data-stu-id="9ecb4-110">Custom settings for Windows 10 devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-windows-10)

[<span data-ttu-id="9ecb4-111">การตั้งค่าแบบกำหนดเองสำหรับ Windows Holographic สำหรับอุปกรณ์ธุรกิจใน Intune</span><span class="sxs-lookup"><span data-stu-id="9ecb4-111">Custom settings for Windows Holographic for Business devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-windows-holographic)