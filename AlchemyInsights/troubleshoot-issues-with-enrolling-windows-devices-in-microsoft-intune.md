---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune
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
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658897"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="7cbe3-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7cbe3-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="7cbe3-103">ตรวจทานแหล่งข้อมูลที่แสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณได้แล้วในตอนนี้</span><span class="sxs-lookup"><span data-stu-id="7cbe3-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="7cbe3-104">ข้อความแสดงข้อผิดพลาดทั่วไปและขั้นตอนการแก้ไข:</span><span class="sxs-lookup"><span data-stu-id="7cbe3-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="7cbe3-105">**ไม่สามารถติดตั้งซอฟต์แวร์ได้ 0x80cf4017:** ใบรับรองบัญชีผู้ใช้ของคุณหมดอายุแล้ว</span><span class="sxs-lookup"><span data-stu-id="7cbe3-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="7cbe3-106">ดาวน์โหลดแพคเกจซอฟต์แวร์ไคลเอ็นต์ของพีซีในคอนโซลผู้ดูแลระบบ Intune อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="7cbe3-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="7cbe3-107">ตรวจทานเอกสารนี้สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="7cbe3-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="7cbe3-108">**รหัสข้อผิดพลาด 0x801c0003:** ข้อผิดพลาดอาจเกิดขึ้นในสถานการณ์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7cbe3-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="7cbe3-109">ผู้ใช้มีอุปกรณ์ที่ลงทะเบียนมากกว่าขีดจำกัดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="7cbe3-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="7cbe3-110">ตรวจทานเอกสารเหล่านี้เพื่อ[เอาอุปกรณ์ออก](https://docs.microsoft.com/intune/devices-wipe)หรือ[เปลี่ยนแปลงขีดจำกัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="7cbe3-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="7cbe3-111">"ผู้ใช้อาจเข้าร่วมอุปกรณ์ใน Azure AD" ถูกตั้งค่าเป็น "ไม่มี"</span><span class="sxs-lookup"><span data-stu-id="7cbe3-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="7cbe3-112">ตั้งค่าเป็นทั้งหมดหรือเลือกผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="7cbe3-112">Set it to all or select users.</span></span> <span data-ttu-id="7cbe3-113">ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="7cbe3-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="7cbe3-114">อุปกรณ์ได้ลงทะเบียนโดยผู้ใช้อื่นแล้ว</span><span class="sxs-lookup"><span data-stu-id="7cbe3-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="7cbe3-115">ถ้าเป็นกรณีนี้ให้เอาอุปกรณ์ออกจากคอนโซล Intune ของ Azure หรือการ unenroll อุปกรณ์ด้วยตนเองก่อนที่จะลองอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="7cbe3-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="7cbe3-116">อุปกรณ์คือ Windows 10 Home</span><span class="sxs-lookup"><span data-stu-id="7cbe3-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="7cbe3-117">เฉพาะ Windows 10 Pro, การศึกษาและ Sku ขององค์กรเท่านั้นที่สามารถเข้าร่วมไดเรกทอรีที่ใช้งานอยู่ของ Azure ได้</span><span class="sxs-lookup"><span data-stu-id="7cbe3-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="7cbe3-118">แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณให้ทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="7cbe3-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="7cbe3-119">ใช้การ [แก้ไขปัญหาของ Intune ของพอร์ทัล](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) เพื่อวินิจฉัยและแก้ไขปัญหาการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="7cbe3-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="7cbe3-120">ตรวจทาน [เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators) สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="7cbe3-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="7cbe3-121">ตรวจทานเอกสารเหล่านี้สำหรับรายการของข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ไขปัญหาแต่ละ[คำแนะนำการแก้ไข](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)ปัญหาและ[เอกสารการแก้ไขปัญหา](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="7cbe3-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="7cbe3-122">[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="7cbe3-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
