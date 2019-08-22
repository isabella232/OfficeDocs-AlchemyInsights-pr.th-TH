---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนสำหรับ DEP ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 3e10f6729d760d9f8f6d04bcb33317fde51a9b80
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507038"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="1285e-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนสำหรับ DEP ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1285e-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="1285e-103">ตรวจทานทรัพยากรแสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณเดี๋ยวนี้</span><span class="sxs-lookup"><span data-stu-id="1285e-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="1285e-104">ถ้าอุปกรณ์ของ DEP จะไม่สามารถลงทะเบียน และเปิดใช้งาน MFA (ด้วยหลายปัจจัยรับรองความถูกต้อง) โปรดปิดใช้งาน MFA</span><span class="sxs-lookup"><span data-stu-id="1285e-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="1285e-105">ขณะนี้ MFA ไม่สนับสนุนสำหรับการลงทะเบียนของ DEP</span><span class="sxs-lookup"><span data-stu-id="1285e-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="1285e-106">ใช้[ไซต์การแก้ไขปัญหาเบื้องต้น Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัย และแก้ปัญหาความล้มเหลวทั่วไปในการลงทะเบียน</span><span class="sxs-lookup"><span data-stu-id="1285e-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="1285e-107">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="1285e-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="1285e-108">ตรวจทานเอกสารเหล่านี้สำหรับรายการของข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ปัญหาแต่ละ:[คำแนะนำในการแก้ไขปัญหา](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)และการ[แก้ไขปัญหาเอกสาร](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="1285e-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="1285e-109">[เรียนรู้เกี่ยวกับโปรแกรมการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)</span><span class="sxs-lookup"><span data-stu-id="1285e-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
