---
title: ใช้Microsoft Intuneพื้นฐานด้านความปลอดภัยเพื่อกําหนดค่าWindows 10อุปกรณ์
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794128"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="dc105-102">ใช้Microsoft Intuneพื้นฐานด้านความปลอดภัยเพื่อกําหนดค่าWindows 10อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="dc105-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="dc105-103">ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัย Intuns ช่วยปกป้องผู้ใช้และอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="dc105-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="dc105-104">ข้อมูลพื้นฐานWindowsกําหนดค่าล่วงหน้าของกลุ่มที่ใช้เพื่อปรับใช้กลุ่มการตั้งค่าที่รู้จักและค่าเริ่มต้นที่แนะWindowsโดยทีมรักษาความปลอดภัยที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="dc105-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="dc105-105">คุณสามารถสร้างเทมเพลตที่ประกอบด้วยโปรไฟล์การกําหนดค่าอุปกรณ์ได้หลายโปรไฟล์ด้วยการสร้างโปรไฟล์ข้อมูลพื้นฐานด้านความปลอดภัยใน Intuny</span><span class="sxs-lookup"><span data-stu-id="dc105-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="dc105-106">เมื่อคุณปรับใช้ข้อมูลพื้นฐานด้านความปลอดภัยกับกลุ่มของผู้ใช้หรืออุปกรณ์ การตั้งค่าจะถูกใช้กับอุปกรณ์ที่เรียกใช้Windows 10 หรือใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="dc105-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="dc105-107">ตัวอย่างเช่น ข้อมูลพื้นฐานเกี่ยวกับการจัดการอุปกรณ์เคลื่อนที่ (MDM) ของ Microsoft จะเปิดใช้งาน BitLocker ไดรฟ์แบบถอดได้โดยอัตโนมัติ ต้องการรหัสผ่านเพื่อปลดล็อกอุปกรณ์ และปิดใช้งานการรับรองความถูกต้องพื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="dc105-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="dc105-108">เมื่อค่าเริ่มต้นใช้ไม่ได้กับสภาพแวดล้อมของคุณ คุณสามารถปรับแต่งข้อมูลพื้นฐานเพื่อปรับใช้การตั้งค่าที่คุณต้องการได้</span><span class="sxs-lookup"><span data-stu-id="dc105-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="dc105-109">ข้อมูลพื้นฐานด้านความปลอดภัยยังช่วยสร้างเวิร์กโฟลว์ที่ปลอดภัยแบบ end-to-end ใน Microsoft 365อีกด้วย</span><span class="sxs-lookup"><span data-stu-id="dc105-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="dc105-110">ข้อมูลพื้นฐานด้านความปลอดภัยมีหลักปฏิบัติที่ดีที่สุดและข้อเสนอแนะเกี่ยวกับการตั้งค่าที่มีผลต่อความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="dc105-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="dc105-111">Intuned ร่วมกับทีมWindowsพื้นฐานที่สร้างข้อมูลพื้นฐานสําหรับนโยบายกลุ่ม ดังนั้นข้อแนะนําเหล่านี้ยึดตามแนวทางที่ทึบและประสบการณ์การใช้งานที่ครอบคลุม</span><span class="sxs-lookup"><span data-stu-id="dc105-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="dc105-112">ถ้าคุณยังใหม่กับ Intun1 และไม่แน่ใจเกี่ยวกับจุดเริ่มต้น การรักษาความปลอดภัยพื้นฐานจะช่วยให้คุณสร้างและปรับใช้โปรไฟล์ที่ปลอดภัยได้อย่างรวดเร็ว</span><span class="sxs-lookup"><span data-stu-id="dc105-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="dc105-113">ถ้าคุณใช้นโยบายกลุ่มในปัจจุบัน การโยกย้ายไปยัง Intuned เพื่อวัตถุประสงค์ในการจัดการจะง่ายขึ้นมากด้วยข้อมูลพื้นฐานด้านความปลอดภัยเนื่องจากข้อมูลเหล่านั้นมีอยู่แล้วใน Intunes และมีความสามารถในการจัดการที่ล้่สุด</span><span class="sxs-lookup"><span data-stu-id="dc105-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="dc105-114">เมื่อต้องการเรียนรู้เพิ่มเติม[ให้ดู Windowsข้อมูลพื้นฐานเกี่ยวกับความปลอดภัย](/windows/security/threat-protection/windows-security-baselines)[และการจัดการอุปกรณ์เคลื่อน](/windows/client-management/mdm/)ที่</span><span class="sxs-lookup"><span data-stu-id="dc105-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

