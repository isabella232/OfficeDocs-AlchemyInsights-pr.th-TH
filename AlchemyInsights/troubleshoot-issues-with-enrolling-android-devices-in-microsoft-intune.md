---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655902"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="b2f16-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b2f16-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="b2f16-103">ตรวจทานทรัพยากรแสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณเดี๋ยวนี้</span><span class="sxs-lookup"><span data-stu-id="b2f16-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="b2f16-104">ปัญหาทั่วไปบางอย่างและขั้นตอนการแก้ปัญหา:</span><span class="sxs-lookup"><span data-stu-id="b2f16-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="b2f16-p101">**อุปกรณ์ไม่เข้ารหัสลับข้อผิดพลาดในเว็บไซต์บริษัท:** รุ่นที่ใหม่กว่าของ Android โดยเฉพาะอย่างยิ่งโดยเริ่มต้น ด้วย v7.0 จำเป็นต้องมีรหัสผ่านการเริ่มต้นระบบเพื่อให้แน่ใจว่า อุปกรณ์ของคุณถูกเข้ารหัสลับทั้งหมด วิธีแก้ไขปัญหาทั่วไปมีการ เปิดใช้งาน pin เริ่มต้นระบบ หรือเข้ารหัสลับอุปกรณ์ได้อย่างสมบูรณ์ ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="b2f16-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="b2f16-p102">**อุปกรณ์ไม่ผ่านการตรวจสอบ ด้วยบริการ Intune หรือแสดงเป็น "Unhealthy" ในคอนโซล admin Intune:** 4.4 บาง Samsung และอุปกรณ์ 5.5 อาจไม่ตรวจสอบถามการบริการ มี 3 วิธีด้วยกันปัญหานี้:</span><span class="sxs-lookup"><span data-stu-id="b2f16-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="b2f16-110">เปิดตัวเว็บไซต์บริษัท Intune แอพลิเคชัน ซึ่งจะเริ่มการซิงค์อุปกรณ์โดยอัตโนมัติด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="b2f16-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="b2f16-111">ปรับปรุงอุปกรณ์ Android 6.0 หรือสูงกว่า</span><span class="sxs-lookup"><span data-stu-id="b2f16-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="b2f16-p103">ปิดใช้งานตัวจัดการสมาร์ท Samsung จากเว็บไซต์บริษัท Intune ในการจัดการ ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)สำหรับรายละเอียดเพิ่มเติมในการตัดสินค้าจากคลังและการแก้ปัญหาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="b2f16-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="b2f16-p104">**ผู้ใช้สิทธิ์การใช้งานชนิดไม่ถูกต้อง**หรือ**ผู้ใช้ไม่รู้จักชื่อข้อผิดพลาด:** ผู้ใช้จำเป็นต้องมอบหมายให้ใบอนุญาต Intune หรือ EMS ตรวจทานเอกสารเหล่านี้เพื่อกำหนดสิทธิ์การใช้งานผ่าน: ศูนย์ดูแล Office หรือ Azure เว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="b2f16-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="b2f16-116">ทรัพยากรเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="b2f16-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="b2f16-p105">ใช้[ไซต์การแก้ไขปัญหาเบื้องต้น Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัย และแก้ปัญหาความล้มเหลวทั่วไปในการลงทะเบียน ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="b2f16-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="b2f16-119">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)สำหรับข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ปัญหาให้กับแต่ละรายการ</span><span class="sxs-lookup"><span data-stu-id="b2f16-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="b2f16-120">[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Android ใน Microsoft Intune](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="b2f16-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

