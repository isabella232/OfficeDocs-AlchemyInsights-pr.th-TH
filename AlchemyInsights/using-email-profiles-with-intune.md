---
title: การใช้โปรไฟล์อีเมลกับ Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653307"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="f5e2c-102">การใช้โปรไฟล์อีเมลกับ Intune</span><span class="sxs-lookup"><span data-stu-id="f5e2c-102">Using email profiles with Intune</span></span>

<span data-ttu-id="f5e2c-103">Intune สามารถใช้ในการสร้างและปรับใช้โปรไฟล์อีเมลสำหรับไคลเอ็นต์อีเมลแบบดั้งเดิม (ภายใน) บนแพลตฟอร์มอุปกรณ์หลายเครื่อง</span><span class="sxs-lookup"><span data-stu-id="f5e2c-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="f5e2c-104">สำหรับข้อมูลเกี่ยวกับข้อจำกัดบางประการที่เกี่ยวข้องกับโปรไฟล์อีเมลรวมถึงวิธีการจัดการการแสดงตนของโปรไฟล์ที่มีอยู่และวิธีการเอาโปรไฟล์อีเมลให้ดู[เพิ่มการตั้งค่าอีเมลไปยังอุปกรณ์โดยใช้ Intune](https://docs.microsoft.com/intune/email-settings-configure)</span><span class="sxs-lookup"><span data-stu-id="f5e2c-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="f5e2c-105">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการสร้างโปรไฟล์อีเมลสำหรับแต่ละแพลตฟอร์มอุปกรณ์ให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="f5e2c-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="f5e2c-106">การตั้งค่าอุปกรณ์ Android เพื่อกำหนดค่าอีเมลการรับรองความถูกต้องและการซิงโครไนซ์ใน Intune</span><span class="sxs-lookup"><span data-stu-id="f5e2c-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="f5e2c-107">เพิ่มการตั้งค่าอีเมลสำหรับอุปกรณ์ iOS และ iPadOS ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f5e2c-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="f5e2c-108">การตั้งค่าโปรไฟล์อีเมลใน Microsoft Intune สำหรับอุปกรณ์ที่ใช้ Windows Phone ๘.๑</span><span class="sxs-lookup"><span data-stu-id="f5e2c-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="f5e2c-109">การตั้งค่าโปรไฟล์อีเมลสำหรับอุปกรณ์ที่ใช้ Windows 10 ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f5e2c-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="f5e2c-110">**ปัญหาการซิงค์ทั่วไป**</span><span class="sxs-lookup"><span data-stu-id="f5e2c-110">**Common syncing issue**</span></span>

<span data-ttu-id="f5e2c-111">**โปรไฟล์อีเมลของ KNOX บน Android จะป้องกันไม่ให้ผู้ติดต่อของผู้ใช้ปฏิทินและงานของผู้ใช้ได้รับการซิงค์กับอุปกรณ์ของผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="f5e2c-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="f5e2c-112">โปรไฟล์อีเมล knox ของ Android ใน Android จะมีตัวเลือกในการตัดสินใจเลือกชนิดเนื้อหาที่จะซิงค์ไปยังอุปกรณ์โดยการตั้งค่าแต่ละรายการที่จะเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="f5e2c-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="f5e2c-113">ถ้าการตั้งค่าสำหรับชนิดเนื้อหาใดๆถูกตั้งค่าเป็น **ไม่ได้กำหนดค่า** (ค่าเริ่มต้น) ชนิดเนื้อหานั้นจะไม่ถูกซิงค์โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="f5e2c-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="f5e2c-114">ผู้ใช้อาจเปิดใช้งานชนิดเนื้อหาที่พวกเขาต้องการโดยตรงในอุปกรณ์ด้วยตนเองแต่การกำหนดค่าดังกล่าวจะถูกเขียนทับโดยการตั้งค่านโยบาย Intune และการหยุดการซิงค์สำหรับชนิดเนื้อหานั้น</span><span class="sxs-lookup"><span data-stu-id="f5e2c-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

