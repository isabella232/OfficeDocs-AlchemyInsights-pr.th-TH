---
title: ข้อผิดพลาดในการซิงค์การลงทะเบียนอุปกรณ์โดยอัตโนมัติของ Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448941"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="14efe-102">ข้อผิดพลาดในการซิงค์การลงทะเบียนอุปกรณ์โดยอัตโนมัติของ Apple</span><span class="sxs-lookup"><span data-stu-id="14efe-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="14efe-103">"เราตรวจพบว่า คุณมีโทเค็น ADE/DEP อย่างน้อยหนึ่งโทเค็นซึ่งอยู่ในสถานะข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="14efe-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="14efe-104">จนกว่าสถานะข้อผิดพลาดจะได้รับการแก้ไขในโทเค็นที่ได้รับผลกระทบแต่ละโทเค็น ฟังก์ชันการฟังก์ชัน ADE จะไม่ผลตามที่คาดไว้"</span><span class="sxs-lookup"><span data-stu-id="14efe-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="14efe-105">ข้อผิดพลาดนี้อาจกรายการด้วยวิธีการต่างๆ รวมถึง:</span><span class="sxs-lookup"><span data-stu-id="14efe-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="14efe-106">อุปกรณ์อาจไม่ซิงค์จาก ABM/ASM ไปยัง Intuns</span><span class="sxs-lookup"><span data-stu-id="14efe-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="14efe-107">การมอบหมายโปรไฟล์การลงทะเบียนอาจล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="14efe-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="14efe-108">อุปกรณ์อาจไม่เสร็จสิ้นการลงทะเบียน ADE</span><span class="sxs-lookup"><span data-stu-id="14efe-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="14efe-109">ตรวจสอบข้อผิดพลาดการซิงค์ที่รายงานในคอนโซล Intuned ภายใต้ **อุปกรณ์ >ลงทะเบียน>การลงทะเบียนของ Apple >โทเค็นโปรแกรมการลงทะเบียน**</span><span class="sxs-lookup"><span data-stu-id="14efe-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="14efe-110">หนึ่งในสาเหตุทั่วไปของข้อผิดพลาดการซิงค์คือหมดอายุของโทเค็นปัจจุบัน</span><span class="sxs-lookup"><span data-stu-id="14efe-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="14efe-111">ในหลายกรณี การต่ออายุโทเค็นที่ได้รับผลกระทบจะแก้ไขปัญหาได้</span><span class="sxs-lookup"><span data-stu-id="14efe-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="14efe-112">ถ้าโทเค็นของคุณอย่างน้อยหนึ่งโทเค็นหมดอายุ แล้ว ให้ดูเอกสารประกอบต่อไปนี้เพื่อช่วยคุณต่ออายุโทเค็นตามความเหมาะสม:</span><span class="sxs-lookup"><span data-stu-id="14efe-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="14efe-113">ต่ออายุโทเค็นการลงทะเบียนอุปกรณ์อัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="14efe-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="14efe-114">นอกจากนี้ คุณสามารถดูคู่มือต่อไปนี้เพื่อดูการแก้ไขที่เป็นไปได้ของข้อผิดพลาดอื่นๆ ที่ทําให้การซิงโครไนซ์โทเค็นล้มเหลว:</span><span class="sxs-lookup"><span data-stu-id="14efe-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="14efe-115">ข้อผิดพลาดในการซิงค์ ABM/ASM ของ iOS/iPadOS และโทเค็นการลงทะเบียนอุปกรณ์อัตโนมัติของ macOS</span><span class="sxs-lookup"><span data-stu-id="14efe-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="14efe-116">ข้อผิดพลาดในการซิงค์ ABM/ASM ของ iOS/iPadOS และโทเค็นการลงทะเบียนอุปกรณ์อัตโนมัติของ macOS</span><span class="sxs-lookup"><span data-stu-id="14efe-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
