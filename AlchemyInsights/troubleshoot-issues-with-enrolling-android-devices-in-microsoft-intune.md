---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intun1
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709017"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="f69ae-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intun1</span><span class="sxs-lookup"><span data-stu-id="f69ae-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="f69ae-103">ตรวจสอบแหล่งข้อมูลที่แสดงอยู่ในรายการด้านล่างเพื่อแก้ไขปัญหาของคุณทันที</span><span class="sxs-lookup"><span data-stu-id="f69ae-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="f69ae-104">ปัญหาทั่วไปและขั้นตอนการแก้ปัญหาบางอย่าง:</span><span class="sxs-lookup"><span data-stu-id="f69ae-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="f69ae-105">**ข้อผิดพลาดอุปกรณ์ไม่เข้ารหัสลับในพอร์ทัลของบริษัท:** Android เวอร์ชันที่ใหม่กว่า โดยเฉพาะอย่างยิ่งเริ่มต้นด้วย v7.0 ต้องใช้รหัสผ่านเริ่มต้นเพื่อให้แน่ใจว่าอุปกรณ์ของคุณได้รับการเข้ารหัสลับอย่างสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="f69ae-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="f69ae-106">วิธีแก้ไขปัญหาทั่วไปคือการเปิดใช้งาน PIN การเริ่มต้นหรือการเข้ารหัสลับอุปกรณ์อย่างสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="f69ae-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="f69ae-107">ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) นี้เพื่อดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="f69ae-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="f69ae-108">**อุปกรณ์ไม่สามารถเช็คอินด้วยบริการ Intun1 หรือแสดงเป็น "ไม่healthy" ในคอนโซลผู้ดูแลระบบ Intun1:** อุปกรณ์ Samsung 4.4 และ 5.5 บางเครื่องอาจไม่ตรวจสอบบริการ</span><span class="sxs-lookup"><span data-stu-id="f69ae-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="f69ae-109">มีวิธีแก้ไขปัญหาที่เป็นไปได้ 3 วิธี:</span><span class="sxs-lookup"><span data-stu-id="f69ae-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="f69ae-110">เปิดแอป Intun1 Company Portal ด้วยตนเอง ซึ่งจะเริ่มการซิงค์อุปกรณ์โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="f69ae-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="f69ae-111">อัปเดตอุปกรณ์เป็น Android 6.0 หรือสูงกว่า</span><span class="sxs-lookup"><span data-stu-id="f69ae-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="f69ae-112">ปิดใช้งาน Samsung Smart Manager จากการจัดการ Intun1 Company Portal</span><span class="sxs-lookup"><span data-stu-id="f69ae-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="f69ae-113">ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) เพื่อดูรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาและการแก้ไขปัญหาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="f69ae-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="f69ae-114">**ข้อผิดพลาดชนิดสิทธิ์การใช้งาน\*\*\*\*ของผู้ใช้ไม่ถูกต้องหรือไม่รู้จักชื่อผู้ใช้:** ผู้ใช้ต้องได้รับการมอบหมายสิทธิ์การใช้งาน Intun1 หรือ EMS</span><span class="sxs-lookup"><span data-stu-id="f69ae-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="f69ae-115">ตรวจทานเอกสารเหล่านี้เพื่อกําหนดสิทธิ์การใช้งานผ่าน: ศูนย์การจัดการ Office หรือพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="f69ae-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="f69ae-116">แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="f69ae-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f69ae-117">ใช้ [พอร์ทัลการแก้ไขปัญหา Intuns](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="f69ae-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f69ae-118">ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune/help-desk-operators) นี้เพื่อดูรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="f69ae-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="f69ae-119">ตรวจทาน [เอกสาร](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) นี้เพื่อดูรายการข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้ลงทะเบียนและแก้ไขปัญหาในแต่ละรายการ</span><span class="sxs-lookup"><span data-stu-id="f69ae-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="f69ae-120">[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intun1](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="f69ae-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
