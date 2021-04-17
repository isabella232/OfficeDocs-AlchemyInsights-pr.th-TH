---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intun1
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823482"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="7c86d-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intun1</span><span class="sxs-lookup"><span data-stu-id="7c86d-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="7c86d-103">ตรวจสอบแหล่งข้อมูลที่แสดงอยู่ด้านล่างเพื่อแก้ไขปัญหาของคุณทันที</span><span class="sxs-lookup"><span data-stu-id="7c86d-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="7c86d-104">ข้อความแสดงข้อผิดพลาดทั่วไปและขั้นตอนการแก้ปัญหามีดังนี้</span><span class="sxs-lookup"><span data-stu-id="7c86d-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="7c86d-105">**ถึงจุดสิ้นสุดอุปกรณ์แล้ว** ผู้ใช้มีอุปกรณ์ที่ลงทะเบียนมากกว่าขีดจํากัดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="7c86d-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="7c86d-106">ตรวจทานเอกสารเหล่านี้[เพื่อเอาอุปกรณ์](https://docs.microsoft.com/intune/devices-wipe)ออก[หรือเปลี่ยนขีดจํากัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="7c86d-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="7c86d-107">**บริการนี้ไม่ได้รับการสนับสนุน ไม่มีนโยบายการลงทะเบียน:** บริการแจ้งแบบพุช (APNS) ของ Apple จะต้องได้รับการกําหนดค่าหรือต่ออายุ</span><span class="sxs-lookup"><span data-stu-id="7c86d-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="7c86d-108">ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) เพื่อดูคําแนะนําเกี่ยวกับวิธีการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="7c86d-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="7c86d-109">**ชนิดสิทธิ์การใช้งานของผู้ใช้ไม่ถูกต้องหรือไม่รู้จักชื่อผู้ใช้:** ผู้ใช้ต้องได้รับการมอบหมายสิทธิ์การใช้งาน Intun1 หรือ EMS</span><span class="sxs-lookup"><span data-stu-id="7c86d-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="7c86d-110">ตรวจทานเอกสารเหล่านี้เพื่อกําหนดสิทธิ์การใช้งานผ่าน:[ศูนย์การจัดการ Office](https://docs.microsoft.com/intune/licenses-assign)หรือ[พอร์ทัล Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="7c86d-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="7c86d-111">แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="7c86d-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="7c86d-112">ใช้ [พอร์ทัลการแก้ไขปัญหา Intun1](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="7c86d-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="7c86d-113">ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune/help-desk-operators) นี้เพื่อดูรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="7c86d-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="7c86d-114">ตรวจทานเอกสารเหล่านี้เพื่อดูรายการข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้การลงทะเบียนและการแก้ไขปัญหาแต่ละรายการ:[คู่มือการแก้ไขปัญหา](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)[และ การแก้ไขปัญหาเอกสาร](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="7c86d-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="7c86d-115">[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intun <2>](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="7c86d-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

