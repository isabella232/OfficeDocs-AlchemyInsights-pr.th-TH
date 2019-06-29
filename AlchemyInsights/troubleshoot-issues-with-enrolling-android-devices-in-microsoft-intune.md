---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367308"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="da7c7-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="da7c7-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="da7c7-103">ตรวจทานทรัพยากรแสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณเดี๋ยวนี้</span><span class="sxs-lookup"><span data-stu-id="da7c7-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="da7c7-104">ปัญหาทั่วไปบางอย่างและขั้นตอนการแก้ปัญหา:</span><span class="sxs-lookup"><span data-stu-id="da7c7-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="da7c7-105">**อุปกรณ์ไม่เข้ารหัสลับข้อผิดพลาดในเว็บไซต์บริษัท:** รุ่นที่ใหม่กว่าของ Android โดยเฉพาะอย่างยิ่งโดยเริ่มต้น ด้วย v7.0 จำเป็นต้องมีรหัสผ่านการเริ่มต้นระบบเพื่อให้แน่ใจว่า อุปกรณ์ของคุณถูกเข้ารหัสลับทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="da7c7-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="da7c7-106">วิธีแก้ไขปัญหาทั่วไปมีการ เปิดใช้งาน pin เริ่มต้นระบบ หรือเข้ารหัสลับอุปกรณ์ได้อย่างสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="da7c7-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="da7c7-107">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="da7c7-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="da7c7-108">**อุปกรณ์ไม่ผ่านการตรวจสอบ ด้วยบริการ Intune หรือแสดงเป็น "Unhealthy" ในคอนโซล admin Intune:** 4.4 บาง Samsung และอุปกรณ์ 5.5 อาจไม่ตรวจสอบถามการบริการ</span><span class="sxs-lookup"><span data-stu-id="da7c7-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="da7c7-109">มี 3 วิธีด้วยกันปัญหานี้:</span><span class="sxs-lookup"><span data-stu-id="da7c7-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="da7c7-110">เปิดตัวเว็บไซต์บริษัท Intune แอพลิเคชัน ซึ่งจะเริ่มการซิงค์อุปกรณ์โดยอัตโนมัติด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="da7c7-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="da7c7-111">ปรับปรุงอุปกรณ์ Android 6.0 หรือสูงกว่า</span><span class="sxs-lookup"><span data-stu-id="da7c7-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="da7c7-112">ปิดใช้งานตัวจัดการสมาร์ท Samsung จากเว็บไซต์บริษัท Intune ในการจัดการ</span><span class="sxs-lookup"><span data-stu-id="da7c7-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="da7c7-113">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)สำหรับรายละเอียดเพิ่มเติมในการตัดสินค้าจากคลังและการแก้ปัญหาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="da7c7-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="da7c7-114">**ผู้ใช้สิทธิ์การใช้งานชนิดไม่ถูกต้อง**หรือ**ผู้ใช้ไม่รู้จักชื่อข้อผิดพลาด:** ผู้ใช้จำเป็นต้องมอบหมายให้ใบอนุญาต Intune หรือ EMS</span><span class="sxs-lookup"><span data-stu-id="da7c7-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="da7c7-115">ตรวจทานเอกสารเหล่านี้เพื่อกำหนดสิทธิ์การใช้งานผ่าน: ศูนย์ดูแล Office หรือ Azure เว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="da7c7-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="da7c7-116">ทรัพยากรเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="da7c7-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="da7c7-117">ใช้[ไซต์การแก้ไขปัญหาเบื้องต้น Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัย และแก้ปัญหาความล้มเหลวทั่วไปในการลงทะเบียน</span><span class="sxs-lookup"><span data-stu-id="da7c7-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="da7c7-118">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="da7c7-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="da7c7-119">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)สำหรับข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ปัญหาให้กับแต่ละรายการ</span><span class="sxs-lookup"><span data-stu-id="da7c7-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="da7c7-120">[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="da7c7-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
