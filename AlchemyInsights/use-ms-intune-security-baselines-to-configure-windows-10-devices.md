---
title: ใช้ Microsoft Intune security ข้อมูลพื้นฐานเพื่อกำหนดค่าอุปกรณ์ Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573786"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="c8fb2-102">ใช้ Microsoft Intune security ข้อมูลพื้นฐานเพื่อกำหนดค่าอุปกรณ์ Windows 10</span><span class="sxs-lookup"><span data-stu-id="c8fb2-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="c8fb2-103">การรักษาความปลอดภัยของ Intune ข้อมูลพื้นฐานช่วยปกป้องผู้ใช้และอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="c8fb2-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="c8fb2-104">ข้อมูลพื้นฐานการตั้งค่าการรักษาความปลอดภัยคือกลุ่มที่กำหนดค่าไว้ล่วงหน้าของ Windows ที่ใช้ในการนำกลุ่มที่รู้จักของการตั้งค่าและค่าเริ่มต้นที่แนะนำโดยทีมความปลอดภัยที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="c8fb2-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="c8fb2-105">ด้วยการสร้างโปรไฟล์หลักของความปลอดภัยใน Intune คุณสามารถสร้างเทมเพลตที่ประกอบด้วยโปรไฟล์การกำหนดค่าอุปกรณ์หลายรายการได้</span><span class="sxs-lookup"><span data-stu-id="c8fb2-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="c8fb2-106">เมื่อคุณปรับใช้ข้อมูลพื้นฐานความปลอดภัยให้กับกลุ่มของผู้ใช้หรืออุปกรณ์การตั้งค่าจะถูกนำไปใช้กับอุปกรณ์ที่ทำงานบน Windows 10 หรือเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="c8fb2-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="c8fb2-107">ตัวอย่างเช่นหลักการรักษาความปลอดภัย MDM โดยอัตโนมัติ (1) เปิดใช้งาน BitLocker สำหรับไดรฟ์แบบถอดได้ (2) จำเป็นต้องใช้รหัสผ่านสำหรับการปลดล็อกอุปกรณ์และ (3) ปิดใช้งานการรับรองความถูกต้องพื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="c8fb2-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="c8fb2-108">เมื่อค่าเริ่มต้นไม่ทำงานสำหรับสภาพแวดล้อมของคุณให้กำหนดข้อมูลพื้นฐานเพื่อนำการตั้งค่าที่คุณต้องการไปใช้</span><span class="sxs-lookup"><span data-stu-id="c8fb2-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="c8fb2-109">การรักษาความปลอดภัยข้อมูลพื้นฐานยังช่วยสร้างเวิร์กโฟลว์ที่มีความปลอดภัยแบบสิ้นสุดสิ้นสุดใน Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="c8fb2-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="c8fb2-110">ต่อไปนี้คือประโยชน์บางประการของสิ่งนี้:</span><span class="sxs-lookup"><span data-stu-id="c8fb2-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="c8fb2-111">หลักปฏิบัติด้านความปลอดภัยมีหลักปฏิบัติที่ดีที่สุดและคำแนะนำสำหรับการตั้งค่าที่มีผลต่อความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="c8fb2-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="c8fb2-112">เนื่องจากคู่ค้า Intune กับทีมการรักษาความปลอดภัยของ Windows ที่สร้างข้อมูลพื้นฐานสำหรับนโยบายกลุ่มคำแนะนำเหล่านี้จะยึดตามคำแนะนำที่เป็นของแข็งและประสบการณ์การใช้งานที่กว้างขวาง</span><span class="sxs-lookup"><span data-stu-id="c8fb2-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="c8fb2-113">ถ้าคุณไม่คุ้นเคยกับ Intune และไม่แน่ใจว่าจะเริ่มต้นที่ไหนแล้วการรักษาความปลอดภัยข้อมูลพื้นฐานจะช่วยให้คุณสามารถสร้างและปรับใช้โปรไฟล์ที่ปลอดภัยได้อย่างรวดเร็ว</span><span class="sxs-lookup"><span data-stu-id="c8fb2-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="c8fb2-114">ถ้าคุณใช้นโยบายกลุ่มอยู่ในขณะนี้ให้โยกย้ายไปยัง Intune เพื่อวัตถุประสงค์ในการจัดการได้ง่ายยิ่งขึ้นด้วยการรักษาความปลอดภัยข้อมูลพื้นฐานเนื่องจากพวกเขาจะถูกสร้างขึ้นใน Intune และรวมถึงความสามารถในการตัดขอบสำหรับการจัดการ</span><span class="sxs-lookup"><span data-stu-id="c8fb2-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="c8fb2-115">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่ [ความปลอดภัยของ Windows ข้อมูลพื้นฐาน](https://go.microsoft.com/fwlink/?linkid=2141503) และ [การจัดการอุปกรณ์เคลื่อน](https://go.microsoft.com/fwlink/?linkid=2141701)ที่</span><span class="sxs-lookup"><span data-stu-id="c8fb2-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>