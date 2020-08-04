---
title: การใช้โปรไฟล์อีเมลกับ Intun
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555759"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="623cc-102">การใช้โปรไฟล์อีเมลกับ Intun</span><span class="sxs-lookup"><span data-stu-id="623cc-102">Using email profiles with Intune</span></span>

<span data-ttu-id="623cc-103">Intunbe สามารถใช้เพื่อสร้างและปรับใช้โปรไฟล์อีเมลสําหรับไคลเอ็นต์อีเมลเนทีฟ (ในตัว) บนแพลตฟอร์มอุปกรณ์หลาย</span><span class="sxs-lookup"><span data-stu-id="623cc-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="623cc-104">สําหรับข้อมูลเกี่ยวกับข้อจํากัดบางอย่างที่เกี่ยวข้องกับโปรไฟล์อีเมล รวมถึงวิธีจัดการการมีอยู่ของโปรไฟล์ที่มีอยู่และวิธีการลบโปรไฟล์อีเมล โปรดดูที่[เพิ่มการตั้งค่าอีเมลไปยังอุปกรณ์ที่ใช้ Intun](https://docs.microsoft.com/intune/email-settings-configure)</span><span class="sxs-lookup"><span data-stu-id="623cc-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="623cc-105">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีสร้างโปรไฟล์อีเมลสําหรับแต่ละแพลตฟอร์มอุปกรณ์ โปรดดู:</span><span class="sxs-lookup"><span data-stu-id="623cc-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="623cc-106">การตั้งค่าอุปกรณ์ Android เพื่อกําหนดค่าอีเมล การตรวจสอบสิทธิ์ และการซิงโครไนซ์ใน Intun</span><span class="sxs-lookup"><span data-stu-id="623cc-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="623cc-107">เพิ่มการตั้งค่าอีเมลสําหรับอุปกรณ์ iOS และ iPadOS ใน Microsoft Intuni</span><span class="sxs-lookup"><span data-stu-id="623cc-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="623cc-108">การตั้งค่าส่วนกําหนดค่าอีเมลใน Microsoft Intun สําหรับอุปกรณ์ที่ใช้ Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="623cc-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="623cc-109">การตั้งค่าส่วนกําหนดค่าอีเมลสําหรับอุปกรณ์ที่ใช้ Windows 10 ใน Microsoft Intun</span><span class="sxs-lookup"><span data-stu-id="623cc-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="623cc-110">**ปัญหาการซิงค์ทั่วไป**</span><span class="sxs-lookup"><span data-stu-id="623cc-110">**Common syncing issue**</span></span>

<span data-ttu-id="623cc-111">**KNOX บนโปรไฟล์อีเมล Android จะป้องกันไม่ให้ผู้ใช้ที่ติดต่อ ปฏิทิน และงาน จากการซิงค์ไปยังอุปกรณ์ของผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="623cc-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="623cc-112">KNOX บนโปรไฟล์อีเมลของ Android KNOX เสนอตัวเลือกสําหรับผู้ดูแลระบบในการตัดสินใจว่าจะซิงค์เนื้อหาประเภทใดไปยังอุปกรณ์โดยการตั้งค่าแต่ละเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="623cc-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="623cc-113">ถ้าการตั้งค่าสําหรับชนิดเนื้อหาใดๆ ถูกตั้งค่าเป็น**ไม่ได้กําหนดค่า**(ค่าเริ่มต้น) ชนิดเนื้อหานั้นจะไม่ซิงค์โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="623cc-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="623cc-114">ผู้ใช้อาจเปิดใช้งานชนิดเนื้อหาที่ต้องการโดยตรงบนอุปกรณ์ด้วยตนเอง แต่การกําหนดค่านั้นถูกเขียนทับโดยการตั้งค่านโยบาย Intun</span><span class="sxs-lookup"><span data-stu-id="623cc-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

