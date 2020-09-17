---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียน DEP ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 50aab6e1e3c0d74d2e305e0bdd47c92b3a27c79f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797315"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="11280-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียน DEP ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="11280-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="11280-103">ตรวจทานแหล่งข้อมูลที่แสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณได้แล้วในตอนนี้</span><span class="sxs-lookup"><span data-stu-id="11280-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="11280-104">ถ้าอุปกรณ์ DEP ไม่สามารถลงทะเบียนและ MFA (การรับรองความถูกต้องแบบหลายปัจจัย) ถูกเปิดใช้งานโปรดปิดใช้งาน MFA</span><span class="sxs-lookup"><span data-stu-id="11280-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="11280-105">ในขณะนี้ MFA ไม่ได้รับการสนับสนุนสำหรับการลงทะเบียน DEP</span><span class="sxs-lookup"><span data-stu-id="11280-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="11280-106">ใช้การ [แก้ไขปัญหาของ Intune ของพอร์ทัล](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขปัญหาการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="11280-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="11280-107">ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators) สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="11280-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="11280-108">ตรวจทานเอกสารเหล่านี้สำหรับรายการของข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ไขปัญหาแต่ละ [คำแนะนำการแก้ไข](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ปัญหาและ [เอกสารการแก้ไขปัญหา](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="11280-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="11280-109">[เรียนรู้เกี่ยวกับโปรแกรมการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)</span><span class="sxs-lookup"><span data-stu-id="11280-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
