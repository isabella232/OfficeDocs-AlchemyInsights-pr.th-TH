---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intun1
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830961"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="741fc-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intun1</span><span class="sxs-lookup"><span data-stu-id="741fc-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="741fc-103">ตรวจสอบแหล่งข้อมูลที่แสดงอยู่ด้านล่างเพื่อแก้ไขปัญหาของคุณทันที</span><span class="sxs-lookup"><span data-stu-id="741fc-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="741fc-104">ปัญหาและขั้นตอนการแก้ปัญหาทั่วไปบางขั้นตอน มีดังนี้</span><span class="sxs-lookup"><span data-stu-id="741fc-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="741fc-105">**ข้อผิดพลาดอุปกรณ์ไม่ได้รับการเข้ารหัสลับในพอร์ทัลของบริษัท:** Android เวอร์ชันที่ใหม่กว่า โดยเฉพาะอย่างยิ่งเริ่มต้นด้วย v7.0 ต้องใช้รหัสผ่านเริ่มต้นเพื่อให้แน่ใจว่าอุปกรณ์ของคุณได้รับการเข้ารหัสลับอย่างสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="741fc-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="741fc-106">โซลูชันทั่วไปคือการเปิดใช้งาน PIN เริ่มต้นหรือเข้ารหัสลับอุปกรณ์อย่างสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="741fc-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="741fc-107">ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) นี้เพื่อดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="741fc-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="741fc-108">**อุปกรณ์ไม่สามารถเช็คอินด้วยบริการ Intun1 หรือแสดงเป็น "ไม่ร้อน" ในคอนโซลผู้ดูแลระบบ Intun1:** อุปกรณ์ Samsung 4.4 และ 5.5 บางรุ่นอาจไม่อยู่ในบริการ</span><span class="sxs-lookup"><span data-stu-id="741fc-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="741fc-109">มี 3 วิธีที่เป็นไปได้ในการแก้ไขปัญหานี้:</span><span class="sxs-lookup"><span data-stu-id="741fc-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="741fc-110">เปิดแอป Intun1 Company Portal ด้วยตนเอง ซึ่งจะเริ่มต้นการซิงค์อุปกรณ์โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="741fc-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="741fc-111">อัปเดตอุปกรณ์เป็น Android 6.0 หรือสูงกว่า</span><span class="sxs-lookup"><span data-stu-id="741fc-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="741fc-112">ปิดใช้งาน Samsung Smart Manager จากการจัดการ Intun1 Company Portal</span><span class="sxs-lookup"><span data-stu-id="741fc-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="741fc-113">ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) เพื่อดูรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาและการแก้ไขปัญหาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="741fc-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="741fc-114">**ชนิดของสิทธิ์การใช้งานของผู้ใช้\*\*\*\*ไม่ถูกต้อง หรือ ชื่อผู้ใช้ไม่รู้จัก ข้อผิดพลาด:** ผู้ใช้ต้องได้รับการมอบหมายสิทธิ์การใช้งาน Intun1 หรือ EMS</span><span class="sxs-lookup"><span data-stu-id="741fc-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="741fc-115">ตรวจทานเอกสารเหล่านี้เพื่อกําหนดสิทธิ์การใช้งานผ่าน: ศูนย์การจัดการ Office หรือพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="741fc-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="741fc-116">แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="741fc-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="741fc-117">ใช้ [พอร์ทัลการแก้ไขปัญหา Intun1](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="741fc-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="741fc-118">ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune/help-desk-operators) นี้เพื่อดูรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="741fc-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="741fc-119">ตรวจทาน [เอกสาร](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) นี้เพื่อดูรายการข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้ลงทะเบียนและแก้ไขปัญหาในแต่ละรายการ</span><span class="sxs-lookup"><span data-stu-id="741fc-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="741fc-120">[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intun1](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="741fc-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
