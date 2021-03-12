---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intun1
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708909"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="b3e81-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intun1</span><span class="sxs-lookup"><span data-stu-id="b3e81-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="b3e81-103">ตรวจสอบแหล่งข้อมูลที่แสดงอยู่ในรายการด้านล่างเพื่อแก้ไขปัญหาของคุณทันที</span><span class="sxs-lookup"><span data-stu-id="b3e81-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="b3e81-104">ข้อความแสดงข้อผิดพลาดทั่วไปและขั้นตอนการแก้ปัญหาบางอย่าง มีดังนี้</span><span class="sxs-lookup"><span data-stu-id="b3e81-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="b3e81-105">**ไม่สามารถติดตั้งซอฟต์แวร์0x80cf4017:** ใบรับรองบัญชีของคุณหมดอายุแล้ว</span><span class="sxs-lookup"><span data-stu-id="b3e81-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="b3e81-106">ดาวน์โหลดแพคเกจซอฟต์แวร์ไคลเอ็นต์พีซีในคอนโซลผู้ดูแลระบบ Intun1 อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="b3e81-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="b3e81-107">ดูเอกสารประกอบนี้เพื่อดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="b3e81-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="b3e81-108">**รหัสข้อผิดพลาด0x801c0003:** ข้อผิดพลาดอาจเกิดขึ้นในสถานการณ์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b3e81-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="b3e81-109">ผู้ใช้ลงทะเบียนอุปกรณ์มากกว่าขีดจํากัดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="b3e81-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="b3e81-110">ตรวจทานเอกสารเหล่านี้ [เพื่อเอาอุปกรณ์](https://docs.microsoft.com/intune/devices-wipe) ออก [หรือเปลี่ยนแปลงขีดจํากัด](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)ของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="b3e81-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="b3e81-111">"ผู้ใช้อาจเข้าร่วมอุปกรณ์ไปยัง Azure AD" ถูกตั้งค่าเป็น "ไม่มี"</span><span class="sxs-lookup"><span data-stu-id="b3e81-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="b3e81-112">ตั้งค่าเป็นผู้ใช้ทั้งหมดหรือเลือกผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="b3e81-112">Set it to all or select users.</span></span> <span data-ttu-id="b3e81-113">ดู [เอกสารประกอบ](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) นี้เพื่อดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="b3e81-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="b3e81-114">อุปกรณ์ได้รับการลงทะเบียนโดยผู้ใช้อื่นแล้ว</span><span class="sxs-lookup"><span data-stu-id="b3e81-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="b3e81-115">ถ้าเป็นกรณีนี้ ให้เอาอุปกรณ์ออกจากคอนโซล Azure Intun1 หรือยกเลิกการลงทะเบียนอุปกรณ์ด้วยตนเองก่อนที่จะลองอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="b3e81-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="b3e81-116">อุปกรณ์ดังกล่าวคือ Windows 10 Home</span><span class="sxs-lookup"><span data-stu-id="b3e81-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="b3e81-117">เฉพาะ Windows 10 Pro, Education และ Enterprise SKU เท่านั้นที่สามารถเข้าร่วม Azure Active Directory ได้</span><span class="sxs-lookup"><span data-stu-id="b3e81-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="b3e81-118">แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="b3e81-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="b3e81-119">ใช้ [พอร์ทัลการแก้ไขปัญหา Intuns](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="b3e81-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b3e81-120">ตรวจทาน [เอกสาร](https://docs.microsoft.com/intune/help-desk-operators) นี้เพื่อดูรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="b3e81-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="b3e81-121">ตรวจทานเอกสารเหล่านี้เพื่อดูรายการข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและการแก้ปัญหา:[คู่มือการแก้ไขปัญหา](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)[และการแก้ไขปัญหาเอกสาร](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="b3e81-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="b3e81-122">[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intun1](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="b3e81-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
