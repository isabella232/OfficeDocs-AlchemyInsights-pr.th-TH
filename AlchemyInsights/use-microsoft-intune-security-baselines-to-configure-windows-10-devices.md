---
title: ใช้ข้อมูลพื้นฐานด้านความปลอดภัยของ Microsoft Intun1 เพื่อกําหนดค่าอุปกรณ์ Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696384"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="4be3d-102">ใช้ข้อมูลพื้นฐานด้านความปลอดภัยของ Microsoft Intun1 ในการกําหนดค่าอุปกรณ์ Windows 10</span><span class="sxs-lookup"><span data-stu-id="4be3d-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="4be3d-103">ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัย Intuns ช่วยปกป้องผู้ใช้และอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="4be3d-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="4be3d-104">ข้อมูลพื้นฐานด้านความปลอดภัยเป็นกลุ่มที่กําหนดค่าล่วงหน้าของ Windows ที่ใช้เพื่อปรับใช้กลุ่มการตั้งค่าที่รู้จักและค่าเริ่มต้นที่แนะนาโดยทีมรักษาความปลอดภัยที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="4be3d-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="4be3d-105">คุณสามารถสร้างเทมเพลตที่ประกอบด้วยโปรไฟล์การกําหนดค่าอุปกรณ์ได้หลายโปรไฟล์โดยการสร้างโปรไฟล์ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัยใน Intunt</span><span class="sxs-lookup"><span data-stu-id="4be3d-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="4be3d-106">เมื่อคุณปรับใช้ข้อมูลพื้นฐานด้านความปลอดภัยกับกลุ่มของผู้ใช้หรืออุปกรณ์ การตั้งค่าจะถูกใช้กับอุปกรณ์ที่เรียกใช้บน Windows 10 หรือเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="4be3d-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="4be3d-107">ตัวอย่างเช่น ข้อมูลพื้นฐานการจัดการอุปกรณ์เคลื่อนที่ของ Microsoft (MDM) โดยอัตโนมัติ (1) เปิดใช้งาน BitLocker บนไดรฟ์แบบถอดได้ (2) ต้องใช้รหัสผ่านในการปลดล็อกอุปกรณ์ และ (3) ปิดใช้งานการรับรองความถูกต้องพื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="4be3d-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="4be3d-108">เมื่อค่าเริ่มต้นไม่ใช้งานกับสภาพแวดล้อมของคุณ คุณสามารถปรับแต่งข้อมูลพื้นฐานเพื่อปรับใช้การตั้งค่าที่คุณต้องการได้</span><span class="sxs-lookup"><span data-stu-id="4be3d-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="4be3d-109">ข้อมูลพื้นฐานด้านความปลอดภัยยังช่วยสร้างเวิร์กโฟลว์ที่ปลอดภัยแบบปลายต่อท้ายใน Microsoft 365 อีกด้วย</span><span class="sxs-lookup"><span data-stu-id="4be3d-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="4be3d-110">ต่อไปนี้เป็นสิทธิประโยชน์บางอย่างของฟังก์ชันการฟังก์ชันนี้:</span><span class="sxs-lookup"><span data-stu-id="4be3d-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="4be3d-111">ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัยมีหลักปฏิบัติที่ดีที่สุดและข้อเสนอแนะในการตั้งค่าที่มีผลต่อความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="4be3d-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="4be3d-112">เนื่องจาก Intun1 ร่วมกับทีมการรักษาความปลอดภัยของ Windows ที่สร้างข้อมูลพื้นฐานสําหรับนโยบายกลุ่ม ข้อแนะนําเหล่านี้ยึดตามแนวทางที่ทึบและประสบการณ์การใช้งานที่ครอบคลุม</span><span class="sxs-lookup"><span data-stu-id="4be3d-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="4be3d-113">ถ้าคุณยังใหม่กับ Intuny และไม่แน่ใจว่าจะเริ่มต้นที่ใด ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัยจะช่วยให้คุณสร้างและปรับใช้โปรไฟล์ที่ปลอดภัยได้อย่างรวดเร็ว</span><span class="sxs-lookup"><span data-stu-id="4be3d-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="4be3d-114">ถ้าคุณยังใช้นโยบายกลุ่มอยู่ การโยกย้ายไปยัง Intunes เพื่อวัตถุประสงค์ในการจัดการจะง่ายยิ่งขึ้นด้วยข้อมูลพื้นฐานเกี่ยวกับความปลอดภัย เนื่องจากข้อมูลพื้นฐานด้านความปลอดภัยเหล่านี้ถูกสร้างขึ้นใน Intunt และมีความสามารถในการจัดการที่ล้าสมัย</span><span class="sxs-lookup"><span data-stu-id="4be3d-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="4be3d-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="4be3d-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>