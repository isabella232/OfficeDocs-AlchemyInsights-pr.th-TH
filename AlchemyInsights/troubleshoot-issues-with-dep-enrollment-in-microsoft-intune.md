---
title: แก้ไขปัญหาการลงทะเบียน DEP ใน Microsoft Intun1
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
ms.openlocfilehash: f76e47c2a3007175ae1bfbd9d20cb59513eb713b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708729"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="031c4-102">แก้ไขปัญหาการลงทะเบียน DEP ใน Microsoft Intun1</span><span class="sxs-lookup"><span data-stu-id="031c4-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="031c4-103">ตรวจสอบแหล่งข้อมูลที่แสดงอยู่ในรายการด้านล่างเพื่อแก้ไขปัญหาของคุณทันที</span><span class="sxs-lookup"><span data-stu-id="031c4-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="031c4-104">ถ้าอุปกรณ์ DEP ไม่สามารถลงทะเบียนและเปิดใช้งาน MFA (การรับรองความถูกต้องโดยใช้หลายปัจจัย) โปรดปิดใช้งาน MFA</span><span class="sxs-lookup"><span data-stu-id="031c4-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="031c4-105">ขณะนี้ MFA ไม่ได้รับการสนับสนุนในการลงทะเบียน DEP</span><span class="sxs-lookup"><span data-stu-id="031c4-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="031c4-106">ใช้ [พอร์ทัลการแก้ไขปัญหา Intuns](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="031c4-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="031c4-107">ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune/help-desk-operators) นี้เพื่อดูรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="031c4-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="031c4-108">ตรวจทานเอกสารเหล่านี้เพื่อดูรายการข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและการแก้ปัญหา: คู่มือ[การแก้ไขปัญหาและ](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)[การแก้ไขปัญหาเอกสาร](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="031c4-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="031c4-109">[เรียนรู้เกี่ยวกับโปรแกรมการลงทะเบียน](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="031c4-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
