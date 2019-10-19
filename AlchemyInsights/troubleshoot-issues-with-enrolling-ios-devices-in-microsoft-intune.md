---
title: แก้ไขปัญหาเกี่ยวกับการทะเบียนอุปกรณ์ iOS ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507022"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="f9d65-102">แก้ไขปัญหาเกี่ยวกับการทะเบียนอุปกรณ์ iOS ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f9d65-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="f9d65-103">ตรวจสอบแหล่งข้อมูลที่แสดงด้านล่างเพื่อแก้ไขปัญหาของคุณตอนนี้</span><span class="sxs-lookup"><span data-stu-id="f9d65-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="f9d65-104">บางข้อความผิดพลาดทั่วไปและขั้นตอนการแก้ปัญหา:</span><span class="sxs-lookup"><span data-stu-id="f9d65-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="f9d65-105">**ถึงฝาอุปกรณ์**แล้ว ผู้ใช้มีอุปกรณ์ที่ลงทะเบียนมากกว่าขีดจำกัดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="f9d65-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="f9d65-106">ตรวจทานเอกสารเหล่านี้เพื่อ[ลบอุปกรณ์](https://docs.microsoft.com/intune/devices-wipe)หรือ[เปลี่ยนขีดจำกัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="f9d65-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="f9d65-107">**บริการนี้ไม่ได้รับการสนับสนุน ไม่มีนโยบายการลงทะเบียน:** บริการแจ้งเตือนแบบพุชของ Apple (APNS) จำเป็นต้องมีการกำหนดค่าหรือต่ออายุ</span><span class="sxs-lookup"><span data-stu-id="f9d65-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="f9d65-108">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)เพื่อดูคำแนะนำในการดำเนินการดังกล่าว</span><span class="sxs-lookup"><span data-stu-id="f9d65-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="f9d65-109">**ประเภทใบอนุญาตของผู้ใช้ไม่ถูกต้องหรือชื่อผู้ใช้ที่ไม่ได้**รับการยอมรับ: ผู้ใช้จำเป็นต้องได้รับใบอนุญาต Intune หรือ EMS</span><span class="sxs-lookup"><span data-stu-id="f9d65-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="f9d65-110">ตรวจทานเอกสารเหล่านี้เพื่อกำหนดสิทธิ์การใช้งานผ่าน:[ศูนย์การจัดการ Office](https://docs.microsoft.com/intune/licenses-assign)หรือ[เว็บไซต์ Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="f9d65-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="f9d65-111">แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="f9d65-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f9d65-112">ใช้การ[แก้ปัญหาเว็บไซต์ Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="f9d65-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f9d65-113">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="f9d65-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="f9d65-114">ตรวจทานเอกสารเหล่านี้สำหรับรายการข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและแก้ปัญหาสำหรับแต่ละ[คำแนะนำการแก้ไขปัญหา](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)และ[เอกสาร](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="f9d65-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="f9d65-115">[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="f9d65-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

