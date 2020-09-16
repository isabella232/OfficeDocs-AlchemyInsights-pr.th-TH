---
title: ใช้โปรไฟล์แบบกำหนดเองใน Intune
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
- "1566"
- "6700005"
ms.openlocfilehash: c3c2233dab60d58438068c6c61a0567b8f68e022
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796595"
---
# <a name="using-custom-policy-in-intune"></a><span data-ttu-id="0704a-102">การใช้นโยบายแบบกำหนดเองใน Intune</span><span class="sxs-lookup"><span data-stu-id="0704a-102">Using custom policy in Intune</span></span>

<span data-ttu-id="0704a-103">Intune มีการตั้งค่าจำนวนมากที่มีอยู่แล้วภายในสำหรับอุปกรณ์ Android, iOS, macOS และ Windows</span><span class="sxs-lookup"><span data-stu-id="0704a-103">Intune has many settings built-in for Android, iOS, macOS and Windows devices.</span></span> <span data-ttu-id="0704a-104">นอกจากนี้คุณยังสามารถสร้างโปรไฟล์แบบกำหนดเองและปรับใช้การตั้งค่าแบบกำหนดเองเหล่านี้กับอุปกรณ์ของคุณได้โดยใช้ Intune</span><span class="sxs-lookup"><span data-stu-id="0704a-104">You can also create a custom profile, and then deploy these custom settings to your devices using Intune.</span></span> <span data-ttu-id="0704a-105">โปรไฟล์แบบกำหนดเองได้รับการออกแบบมาเพื่อเพิ่มการตั้งค่าอุปกรณ์และฟีเจอร์ที่ไม่ได้มีอยู่แล้วใน Windows Intune</span><span class="sxs-lookup"><span data-stu-id="0704a-105">Custom profiles are designed to add device settings and features that aren't built in to Intune.</span></span>

[<span data-ttu-id="0704a-106">การตั้งค่าแบบกำหนดเองสำหรับอุปกรณ์ Android ใน Intune</span><span class="sxs-lookup"><span data-stu-id="0704a-106">Custom settings for Android devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-android)

[<span data-ttu-id="0704a-107">การตั้งค่าแบบกำหนดเองสำหรับอุปกรณ์ Android สำหรับองค์กรใน Intune</span><span class="sxs-lookup"><span data-stu-id="0704a-107">Custom settings for Android Enterprise devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-android-for-work)

[<span data-ttu-id="0704a-108">การตั้งค่าแบบกำหนดเองสำหรับอุปกรณ์ iOS ใน Intune</span><span class="sxs-lookup"><span data-stu-id="0704a-108">Custom settings for iOS devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-ios)

[<span data-ttu-id="0704a-109">การตั้งค่าแบบกำหนดเองสำหรับอุปกรณ์ macOS ใน Intune</span><span class="sxs-lookup"><span data-stu-id="0704a-109">Custom settings for macOS devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-macos)

[<span data-ttu-id="0704a-110">การตั้งค่าแบบกำหนดเองสำหรับอุปกรณ์ Windows 10 ใน Intune</span><span class="sxs-lookup"><span data-stu-id="0704a-110">Custom settings for Windows 10 devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-windows-10)

[<span data-ttu-id="0704a-111">การตั้งค่าแบบกำหนดเองสำหรับอุปกรณ์ Windows โฮโลแกรมสำหรับธุรกิจใน Intune</span><span class="sxs-lookup"><span data-stu-id="0704a-111">Custom settings for Windows Holographic for Business devices in Intune</span></span>](https://docs.microsoft.com/intune/custom-settings-windows-holographic)