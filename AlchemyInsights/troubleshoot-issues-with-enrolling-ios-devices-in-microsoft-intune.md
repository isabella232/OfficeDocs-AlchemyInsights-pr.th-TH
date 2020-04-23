---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736177"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="9f29b-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9f29b-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="9f29b-103">ตรวจสอบทรัพยากรที่แสดงด้านล่างเพื่อแก้ไขปัญหาของคุณตอนนี้</span><span class="sxs-lookup"><span data-stu-id="9f29b-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="9f29b-104">ข้อความแสดงข้อผิดพลาดและขั้นตอนการแก้ปัญหาที่พบบ่อย:</span><span class="sxs-lookup"><span data-stu-id="9f29b-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="9f29b-105">**ถึงอุปกรณ์แล้ว** ผู้ใช้มีอุปกรณ์ที่ลงทะเบียนมากกว่าขีดจํากัดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="9f29b-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="9f29b-106">ตรวจสอบเอกสารเหล่านี้เพื่อ[เอาอุปกรณ์](https://docs.microsoft.com/intune/devices-wipe)ออก หรือ[เปลี่ยนขีดจํากัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="9f29b-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="9f29b-107">**บริการนี้ไม่ได้รับการสนับสนุน ไม่มีนโยบายการลงทะเบียน:** บริการแจ้งเตือนแบบพุชของ Apple (APNS) จําเป็นต้องได้รับการกําหนดค่าหรือต่ออายุ</span><span class="sxs-lookup"><span data-stu-id="9f29b-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="9f29b-108">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)สําหรับคําแนะนําเกี่ยวกับวิธีการทําเช่นนั้น</span><span class="sxs-lookup"><span data-stu-id="9f29b-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="9f29b-109">**ชนิดสิทธิ์การใช้งานของผู้ใช้ไม่ถูกต้องหรือชื่อผู้ใช้ที่ไม่รู้จัก:** ผู้ใช้จําเป็นต้องได้รับใบอนุญาต Intune หรือ EMS</span><span class="sxs-lookup"><span data-stu-id="9f29b-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="9f29b-110">ตรวจทานเอกสารเหล่านี้เพื่อกําหนดสิทธิ์การใช้งานผ่าน[: ศูนย์การจัดการ Office](https://docs.microsoft.com/intune/licenses-assign)หรือพอร์ทัล[Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="9f29b-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="9f29b-111">ทรัพยากรเพิ่มเติมเพื่อช่วยแก้ปัญหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="9f29b-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="9f29b-112">ใช้[การแก้ไขปัญหาเว็บไซต์ Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัยและแก้ไขปัญหาความล้มเหลวในการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="9f29b-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9f29b-113">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สําหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="9f29b-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="9f29b-114">ตรวจทานเอกสารเหล่านี้เพื่อดูรายการของข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้การลงทะเบียนและวิธีแก้ปัญหาแต่ละรายการ:[คู่มือการแก้ไขปัญหา](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)และ[เอกสารการแก้ไขปัญหา](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="9f29b-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="9f29b-115">[เรียนรู้วิธีลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="9f29b-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

