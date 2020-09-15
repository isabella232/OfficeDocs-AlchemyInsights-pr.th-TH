---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689973"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="65b59-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="65b59-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="65b59-103">ตรวจทานแหล่งข้อมูลที่แสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณได้แล้วในตอนนี้</span><span class="sxs-lookup"><span data-stu-id="65b59-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="65b59-104">ปัญหาทั่วไปและขั้นตอนการแก้ไขปัญหาบางอย่าง:</span><span class="sxs-lookup"><span data-stu-id="65b59-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="65b59-105">**ไม่มีข้อผิดพลาดในการเข้ารหัสลับอุปกรณ์ในพอร์ทัลของบริษัท:** เวอร์ชันที่ใหม่กว่าของ Android โดยเฉพาะอย่างยิ่งเริ่มต้นด้วย v 7.0 จำเป็นต้องใช้รหัสผ่านเริ่มต้นเพื่อตรวจสอบให้แน่ใจว่าอุปกรณ์ของคุณได้รับการเข้ารหัสลับทั้งหมดแล้ว</span><span class="sxs-lookup"><span data-stu-id="65b59-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="65b59-106">วิธีแก้ไขปัญหาทั่วไปคือการเปิดใช้งาน pin เริ่มต้นระบบหรือเข้ารหัสลับอุปกรณ์ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="65b59-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="65b59-107">ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="65b59-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="65b59-108">**อุปกรณ์ล้มเหลวในการเช็คอินด้วยบริการ Intune หรือแสดงเป็น "ไม่แข็งแรง" ในคอนโซลผู้ดูแลระบบ Intune:** อุปกรณ์ Samsung ๔.๔และ๕.๕บางรายการอาจไม่สามารถตรวจสอบได้ในบริการ</span><span class="sxs-lookup"><span data-stu-id="65b59-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="65b59-109">มีวิธีแก้ไขปัญหาที่เป็นไปได้3วิธีดังนี้</span><span class="sxs-lookup"><span data-stu-id="65b59-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="65b59-110">เปิดแอป Intune ของพอร์ทัลของบริษัท Intune ด้วยตนเองซึ่งจะเริ่มการซิงค์อุปกรณ์โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="65b59-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="65b59-111">อัปเดตอุปกรณ์ไปยัง Android ๖.๐หรือสูงกว่า</span><span class="sxs-lookup"><span data-stu-id="65b59-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="65b59-112">ปิดใช้งานตัวจัดการสมาร์ทโฟนของ Samsung จากการจัดการพอร์ทัลบริษัท Intune</span><span class="sxs-lookup"><span data-stu-id="65b59-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="65b59-113">ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาและวิธีแก้ไขปัญหาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="65b59-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="65b59-114">**ชนิดสิทธิ์การใช้งานของผู้ใช้\*\*\*\*ไม่ได้รับการยอมรับข้อผิดพลาด:** ผู้ใช้ที่จำเป็นต้องได้รับการกำหนดสิทธิ์การใช้งาน Intune หรือ EMS</span><span class="sxs-lookup"><span data-stu-id="65b59-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="65b59-115">ตรวจทานเอกสารเหล่านี้เพื่อมอบหมายสิทธิ์การใช้งานผ่าน: ศูนย์การจัดการ Office หรือพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="65b59-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="65b59-116">แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณให้ทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="65b59-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="65b59-117">ใช้การ [แก้ไขปัญหาของ Intune ของพอร์ทัล](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขปัญหาการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="65b59-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="65b59-118">ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators) สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="65b59-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="65b59-119">ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) สำหรับรายการของข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ไขปัญหาแต่ละรายการ</span><span class="sxs-lookup"><span data-stu-id="65b59-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="65b59-120">[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="65b59-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
