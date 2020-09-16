---
title: Pin ของอุปกรณ์/การตั้งค่ารหัสผ่านใหม่จาก Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1278"
- "6700008"
ms.openlocfilehash: 66255fc87a55161158aa4121d68d7ccd04b552ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731018"
---
# <a name="device-pinpassword-reset-from-intune"></a><span data-ttu-id="7a968-102">Pin ของอุปกรณ์/การตั้งค่ารหัสผ่านใหม่จาก Intune</span><span class="sxs-lookup"><span data-stu-id="7a968-102">Device pin/password reset from Intune</span></span>

<span data-ttu-id="7a968-103">คุณสามารถเอารหัสผ่านหรือบังคับให้ผู้ใช้สร้างรหัสผ่านใหม่ใน Intune สำหรับอุปกรณ์ที่ใช้ iOS หรือ Android โดยใช้การดำเนินการเอารหัสผ่านออก</span><span class="sxs-lookup"><span data-stu-id="7a968-103">You can remove a passcode or force a user to create a new passcode in Intune for a device running iOS or Android by using the Remove Passcode action.</span></span>

<span data-ttu-id="7a968-104">ชนิดของระบบปฏิบัติการที่เฉพาะเจาะจงและชนิดโปรไฟล์การทำงานสนับสนุนการกระทำนี้เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="7a968-104">Only specific operating system types and work profile types support this action.</span></span>

<span data-ttu-id="7a968-105">สำหรับรายละเอียดเกี่ยวกับแพลตฟอร์มที่ได้รับการสนับสนุนและวิธีการเรียกใช้การดำเนินการตั้งค่ารหัสผ่านใหม่ให้ดูที่ [ตั้งค่าใหม่หรือเอารหัสผ่านอุปกรณ์ใน Intune](https://docs.microsoft.com/intune/device-passcode-reset)ออก</span><span class="sxs-lookup"><span data-stu-id="7a968-105">For details about supported platforms and how to trigger the reset passcode action, see [Reset or remove a device passcode in Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span></span>

<span data-ttu-id="7a968-106">คุณสามารถตั้งค่า pin ที่มีอยู่ใหม่ให้เป็นค่าใหม่โดยใช้การดำเนินการตั้งค่า Pin ใหม่บนอุปกรณ์ที่ใช้ระบบปฏิบัติการ Windows 10 บนอุปกรณ์เคลื่อนที่</span><span class="sxs-lookup"><span data-stu-id="7a968-106">You can reset an existing pin to a new value using the Pin Reset action on devices running the Windows 10 Mobile operating system.</span></span> <span data-ttu-id="7a968-107">การทำเช่นนี้จะช่วยให้ผู้ใช้สามารถปลดล็อกอุปกรณ์และตั้งค่า pin ใหม่ได้ตามความเหมาะสม</span><span class="sxs-lookup"><span data-stu-id="7a968-107">This allows the user to unlock the device and set a new pin as appropriate.</span></span> <span data-ttu-id="7a968-108">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ตั้งค่ารหัสผ่านใหม่บนอุปกรณ์ Windows โดยใช้ Intune](https://docs.microsoft.com/intune/device-windows-pin-reset)</span><span class="sxs-lookup"><span data-stu-id="7a968-108">For more info, see [Reset the passcode on Windows devices using Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span></span>