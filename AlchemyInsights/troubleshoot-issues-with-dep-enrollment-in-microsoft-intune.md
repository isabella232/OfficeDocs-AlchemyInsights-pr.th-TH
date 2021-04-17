---
title: แก้ไขปัญหาการลงทะเบียน DEP ใน Microsoft Intun1
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 27abeafba5588ca74569ba6bebc5d940b767ea3f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824526"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="bd61c-102">แก้ไขปัญหาการลงทะเบียน DEP ใน Microsoft Intun1</span><span class="sxs-lookup"><span data-stu-id="bd61c-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="bd61c-103">ตรวจสอบแหล่งข้อมูลที่แสดงอยู่ด้านล่างเพื่อแก้ไขปัญหาของคุณทันที</span><span class="sxs-lookup"><span data-stu-id="bd61c-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="bd61c-104">ถ้าอุปกรณ์ DEP ไม่สามารถลงทะเบียนและเปิดใช้งาน MFA (การรับรองความถูกต้องโดยใช้หลายปัจจัย) โปรดปิดใช้งาน MFA</span><span class="sxs-lookup"><span data-stu-id="bd61c-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="bd61c-105">ขณะนี้ MFA ไม่ได้รับการสนับสนุนในการลงทะเบียน DEP</span><span class="sxs-lookup"><span data-stu-id="bd61c-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="bd61c-106">ใช้ [พอร์ทัลการแก้ไขปัญหา Intun1](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="bd61c-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="bd61c-107">ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune/help-desk-operators) นี้เพื่อดูรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="bd61c-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="bd61c-108">ตรวจทานเอกสารเหล่านี้เพื่อดูรายการข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้การลงทะเบียนและการแก้ไขปัญหาแต่ละรายการ: คู่มือ [การแก้ไขปัญหา](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) และ [การแก้ไขปัญหาเอกสาร](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="bd61c-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="bd61c-109">[เรียนรู้เกี่ยวกับโปรแกรมการลงทะเบียน](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="bd61c-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
