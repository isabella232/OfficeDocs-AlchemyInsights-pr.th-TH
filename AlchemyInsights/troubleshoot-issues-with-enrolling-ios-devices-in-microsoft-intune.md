---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507022"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="4b0aa-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4b0aa-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="4b0aa-103">ตรวจทานทรัพยากรแสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณเดี๋ยวนี้</span><span class="sxs-lookup"><span data-stu-id="4b0aa-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="4b0aa-104">ข้อผิดพลาดทั่วไปบางอย่างและขั้นตอนการแก้ปัญหา:</span><span class="sxs-lookup"><span data-stu-id="4b0aa-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="4b0aa-105">**ทุนอุปกรณ์ที่มาถึง** ผู้ใช้มีอุปกรณ์เพิ่มเติมที่ลงทะเบียนไว้เกินขีดจำกัดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="4b0aa-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="4b0aa-106">ตรวจทานเอกสารเหล่านี้เมื่อต้องการ[เอาอุปกรณ์ออก](https://docs.microsoft.com/intune/devices-wipe)หรือ[เปลี่ยนแปลงขีดจำกัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="4b0aa-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="4b0aa-107">**บริการนี้ไม่ได้รับการสนับสนุน นโยบายไม่มีการลงทะเบียน:** Apple ดันแจ้งเตือนบริการ (APNS) ที่จำเป็นต้องมีการตั้งค่าคอนฟิก หรือต่ออายุ</span><span class="sxs-lookup"><span data-stu-id="4b0aa-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="4b0aa-108">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)สำหรับคำแนะนำเกี่ยวกับวิธีการทำเช่นนั้น</span><span class="sxs-lookup"><span data-stu-id="4b0aa-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="4b0aa-109">**ไม่ถูกต้องชนิดลิขสิทธิ์ของผู้ใช้หรือชื่อผู้ใช้ที่ไม่รู้จัก:** ผู้ใช้อาจต้องการกำหนดใบอนุญาต Intune หรือ EMS</span><span class="sxs-lookup"><span data-stu-id="4b0aa-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="4b0aa-110">ตรวจทานเอกสารเหล่านี้เพื่อกำหนดสิทธิ์การใช้งานผ่าน:[ศูนย์ดูแล Office](https://docs.microsoft.com/intune/licenses-assign)หรือ[Azure เว็บไซต์](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="4b0aa-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="4b0aa-111">ทรัพยากรเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="4b0aa-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="4b0aa-112">ใช้[ไซต์การแก้ไขปัญหาเบื้องต้น Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัย และแก้ปัญหาความล้มเหลวทั่วไปในการลงทะเบียน</span><span class="sxs-lookup"><span data-stu-id="4b0aa-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="4b0aa-113">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="4b0aa-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="4b0aa-114">ตรวจทานเอกสารเหล่านี้สำหรับรายการของข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ปัญหาแต่ละ:[คำแนะนำในการแก้ไขปัญหา](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)และการ[แก้ไขปัญหาเอกสาร](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="4b0aa-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="4b0aa-115">[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ iOS ใน Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="4b0aa-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

