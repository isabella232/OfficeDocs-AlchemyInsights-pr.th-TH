---
title: อุปกรณ์ pin / รหัสผ่านรีเซ็ตจาก Intun
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1278"
- "6700008"
ms.openlocfilehash: fd3bb957b0da22dfab5a9988a82e398757e12ee5
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440095"
---
# <a name="device-pinpassword-reset-from-intune"></a><span data-ttu-id="611ef-102">อุปกรณ์ pin / รหัสผ่านรีเซ็ตจาก Intun</span><span class="sxs-lookup"><span data-stu-id="611ef-102">Device pin/password reset from Intune</span></span>

<span data-ttu-id="611ef-103">คุณสามารถลบรหัสผ่านหรือบังคับให้ผู้ใช้สร้างรหัสผ่านใหม่ใน Intuner สําหรับอุปกรณ์ที่ใช้ iOS หรือ Android โดยใช้การกระทําเอารหัสออก</span><span class="sxs-lookup"><span data-stu-id="611ef-103">You can remove a passcode or force a user to create a new passcode in Intune for a device running iOS or Android by using the Remove Passcode action.</span></span>

<span data-ttu-id="611ef-104">เฉพาะชนิดระบบปฏิบัติการและประเภทโปรไฟล์งานเฉพาะเท่านั้นที่สนับสนุนการดําเนินการนี้</span><span class="sxs-lookup"><span data-stu-id="611ef-104">Only specific operating system types and work profile types support this action.</span></span>

<span data-ttu-id="611ef-105">สําหรับรายละเอียดเกี่ยวกับแพลตฟอร์มที่สนับสนุนและวิธีการทริกเกอร์การดําเนินการรีเซ็ตรหัสผ่าน ให้ดูที่[รีเซ็ตหรือเอารหัสผ่านอุปกรณ์ใน Intun](https://docs.microsoft.com/intune/device-passcode-reset)</span><span class="sxs-lookup"><span data-stu-id="611ef-105">For details about supported platforms and how to trigger the reset passcode action, see [Reset or remove a device passcode in Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span></span>

<span data-ttu-id="611ef-106">คุณสามารถตั้งค่าหมุดที่มีอยู่เป็นค่าใหม่โดยใช้การกระทํา Pin Reset บนอุปกรณ์ที่ใช้ระบบปฏิบัติการ Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="611ef-106">You can reset an existing pin to a new value using the Pin Reset action on devices running the Windows 10 Mobile operating system.</span></span> <span data-ttu-id="611ef-107">วิธีนี้ช่วยให้ผู้ใช้สามารถปลดล็อกอุปกรณ์และตั้งหมุดใหม่ตามความเหมาะสม</span><span class="sxs-lookup"><span data-stu-id="611ef-107">This allows the user to unlock the device and set a new pin as appropriate.</span></span> <span data-ttu-id="611ef-108">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[รีเซ็ตรหัสผ่านบนอุปกรณ์ Windows โดยใช้ Intun](https://docs.microsoft.com/intune/device-windows-pin-reset)</span><span class="sxs-lookup"><span data-stu-id="611ef-108">For more info, see [Reset the passcode on Windows devices using Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span></span>