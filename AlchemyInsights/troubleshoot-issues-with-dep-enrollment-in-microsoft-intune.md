---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียน DEP ในอินจูนของ Microsoft
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 11b0d73c34996fd84431b38d77b64536d386977e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766728"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="f6b04-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียน DEP ในอินจูนของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="f6b04-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="f6b04-103">ตรวจสอบทรัพยากรที่แสดงด้านล่างเพื่อแก้ไขปัญหาของคุณตอนนี้</span><span class="sxs-lookup"><span data-stu-id="f6b04-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="f6b04-104">ถ้าอุปกรณ์ DEP ไม่สามารถลงทะเบียนได้ และเปิดใช้งาน MFA (การตรวจสอบด้วยหลายปัจจัย) โปรดปิดใช้งาน MFA</span><span class="sxs-lookup"><span data-stu-id="f6b04-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="f6b04-105">ขณะนี้ MFA ไม่ได้รับการสนับสนุนสําหรับการลงทะเบียน DEP</span><span class="sxs-lookup"><span data-stu-id="f6b04-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="f6b04-106">ใช้[การแก้ไขปัญหาเว็บไซต์ Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัยและแก้ไขปัญหาความล้มเหลวในการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="f6b04-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f6b04-107">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สําหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="f6b04-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="f6b04-108">ตรวจทานเอกสารเหล่านี้เพื่อดูรายการข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้การลงทะเบียนและวิธีแก้ปัญหาแต่ละรายการ:[คู่มือการแก้ไขปัญหา](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)และ[เอกสารการแก้ไขปัญหา](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="f6b04-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="f6b04-109">[เรียนรู้เกี่ยวกับโปรแกรมการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)</span><span class="sxs-lookup"><span data-stu-id="f6b04-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
