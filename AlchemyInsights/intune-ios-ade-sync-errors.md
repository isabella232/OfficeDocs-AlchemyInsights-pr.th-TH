---
title: ข้อผิดพลาดการซิงค์การลงทะเบียนอุปกรณ์อัตโนมัติของ Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714973"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="b9bfe-102">ข้อผิดพลาดการซิงค์การลงทะเบียนอุปกรณ์อัตโนมัติของ Apple</span><span class="sxs-lookup"><span data-stu-id="b9bfe-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="b9bfe-103">"เราตรวจพบว่าคุณมีโทเค็น ADE/DEP อย่างน้อยหนึ่งโทเค็นที่อยู่ในสถานะข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="b9bfe-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="b9bfe-104">จนกว่าสถานะข้อผิดพลาดจะได้รับการแก้ไขสำหรับโทเค็นที่ได้รับผลกระทบแต่ละรายการฟังก์ชัน ADE จะไม่ทำงานให้เหมือนกัน "</span><span class="sxs-lookup"><span data-stu-id="b9bfe-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="b9bfe-105">ข้อผิดพลาดนี้อาจแสดงรายการในหลายวิธีรวมถึง:</span><span class="sxs-lookup"><span data-stu-id="b9bfe-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="b9bfe-106">อุปกรณ์อาจไม่ซิงค์จากการ .ABM/ASM ไปยัง Intune</span><span class="sxs-lookup"><span data-stu-id="b9bfe-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="b9bfe-107">งานที่มอบหมายโปรไฟล์การลงทะเบียนอาจล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="b9bfe-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="b9bfe-108">อุปกรณ์อาจไม่เสร็จสมบูรณ์การลงทะเบียน ADE เสร็จเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="b9bfe-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="b9bfe-109">ตรวจหาข้อผิดพลาดในการซิงค์ที่รายงานในคอนโซล Intune ภายใต้ **อุปกรณ์ > การลงทะเบียนอุปกรณ์ > การลงทะเบียน Apple > โทเค็นโปรแกรมการลง** ทะเบียนและตรวจทานเอกสารต่อไปนี้เพื่อดูสิ่งที่อาจเกิดขึ้น:</span><span class="sxs-lookup"><span data-stu-id="b9bfe-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="b9bfe-110">ข้อผิดพลาดการซิงค์ของ .ABM/ASM สำหรับ iOS/iPadOS และ macOS โทเค็นการลงทะเบียนอุปกรณ์อัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="b9bfe-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
