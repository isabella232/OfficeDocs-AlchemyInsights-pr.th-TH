---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759639"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="36804-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="36804-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="36804-103">ตรวจสอบทรัพยากรที่แสดงด้านล่างเพื่อแก้ไขปัญหาของคุณตอนนี้</span><span class="sxs-lookup"><span data-stu-id="36804-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="36804-104">ปัญหาทั่วไปและขั้นตอนการแก้ปัญหา:</span><span class="sxs-lookup"><span data-stu-id="36804-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="36804-105">**ข้อผิดพลาดที่เข้ารหัสลับอุปกรณ์ในพอร์ทัลของบริษัท:** เวอร์ชันใหม่ของ Android โดยเฉพาะอย่างยิ่งเริ่มต้นด้วย v7.0 ต้องใช้รหัสผ่านเริ่มต้นเพื่อให้แน่ใจว่าอุปกรณ์ของคุณมีการเข้ารหัสอย่างเต็มที่</span><span class="sxs-lookup"><span data-stu-id="36804-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="36804-106">โซลูชันทั่วไปคือการเปิดใช้งาน pin เริ่มต้นระบบ หรือเข้ารหัสลับอุปกรณ์ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="36804-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="36804-107">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="36804-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="36804-108">**อุปกรณ์ไม่สามารถเช็คอินด้วยบริการ Intune หรือแสดงเป็น "ไม่แข็งแรง" ในคอนโซลผู้ดูแลระบบ Intune:** อุปกรณ์บางตัวของ Samsung 4.4 และ 5.5 อาจไม่เช็คอินบริการ</span><span class="sxs-lookup"><span data-stu-id="36804-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="36804-109">มี 3 วิธีแก้ไขปัญหาที่เป็นไปได้สําหรับปัญหานี้:</span><span class="sxs-lookup"><span data-stu-id="36804-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="36804-110">เปิดแอปเว็บไซต์ของบริษัท Intune ด้วยตนเอง ซึ่งจะเริ่มต้นการซิงค์อุปกรณ์โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="36804-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="36804-111">อัปเดตอุปกรณ์เป็น Android 6.0 หรือสูงกว่า</span><span class="sxs-lookup"><span data-stu-id="36804-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="36804-112">ปิดใช้งานตัวจัดการสมาร์ทของ Samsung จากการจัดการเว็บไซต์บริษัท Intune</span><span class="sxs-lookup"><span data-stu-id="36804-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="36804-113">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาและวิธีแก้ปัญหาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="36804-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="36804-114">**ชนิดสิทธิ์การใช้งานของผู้ใช้ไม่ถูกต้อง**หรือ**ชื่อผู้ใช้ที่ไม่รู้จักข้อผิดพลาด:** ผู้ใช้จําเป็นต้องกําหนดสิทธิ์การใช้งาน Intune หรือ EMS</span><span class="sxs-lookup"><span data-stu-id="36804-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="36804-115">ตรวจทานเอกสารเหล่านี้เพื่อกําหนดสิทธิ์การใช้งานผ่าน: ศูนย์การจัดการ Office หรือพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="36804-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="36804-116">ทรัพยากรเพิ่มเติมเพื่อช่วยแก้ปัญหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="36804-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="36804-117">ใช้[การแก้ไขปัญหาเว็บไซต์ Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัยและแก้ไขปัญหาความล้มเหลวในการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="36804-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="36804-118">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สําหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="36804-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="36804-119">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)เพื่อดูรายการของข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้การลงทะเบียนและวิธีแก้ปัญหาในแต่ละรายการ</span><span class="sxs-lookup"><span data-stu-id="36804-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="36804-120">[เรียนรู้วิธีการลงทะเบียนอุปกรณ์แอนดรอยด์ใน Microsoft Intune](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="36804-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
