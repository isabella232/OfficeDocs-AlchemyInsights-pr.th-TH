---
title: การแก้ไขปัญหาเกี่ยวกับการทะเบียนอุปกรณ์ Windows ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665851"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="a156a-102">การแก้ไขปัญหาเกี่ยวกับการทะเบียนอุปกรณ์ Windows ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a156a-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="a156a-103">ตรวจสอบแหล่งข้อมูลที่แสดงด้านล่างเพื่อแก้ไขปัญหาของคุณตอนนี้</span><span class="sxs-lookup"><span data-stu-id="a156a-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="a156a-104">บางข้อความผิดพลาดทั่วไปและขั้นตอนการแก้ปัญหา:</span><span class="sxs-lookup"><span data-stu-id="a156a-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="a156a-105">**ซอฟต์แวร์ไม่สามารถติดตั้ง, 0x80cf4017:** ใบรับรองบัญชีของคุณหมดอายุแล้ว</span><span class="sxs-lookup"><span data-stu-id="a156a-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="a156a-106">ดาวน์โหลดแพคเกจซอฟต์แวร์ไคลเอ็นต์คอมพิวเตอร์อีกครั้งในคอนโซลการดูแล Intune</span><span class="sxs-lookup"><span data-stu-id="a156a-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="a156a-107">ตรวจทานเอกสารฉบับนี้สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="a156a-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="a156a-108">**รหัสข้อผิดพลาด 0x801c0003:** ข้อผิดพลาดสามารถเกิดขึ้นได้ในสถานการณ์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a156a-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="a156a-109">ผู้ใช้มีอุปกรณ์ที่ลงทะเบียนมากกว่าขีดจำกัดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="a156a-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="a156a-110">ตรวจทานเอกสารเหล่านี้เพื่อ[ลบอุปกรณ์](https://docs.microsoft.com/intune/devices-wipe)หรือ[เปลี่ยนขีดจำกัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="a156a-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="a156a-111">"ผู้ใช้อาจเข้าร่วมอุปกรณ์กับโฆษณา Azure" ถูกตั้งค่าเป็น "ไม่มี"</span><span class="sxs-lookup"><span data-stu-id="a156a-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="a156a-112">ตั้งค่าให้ทั้งหมดหรือเลือกผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="a156a-112">Set it to all or select users.</span></span> <span data-ttu-id="a156a-113">ตรวจทาน[เอกสารประกอบนี้](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="a156a-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="a156a-114">อุปกรณ์ได้ลงทะเบียนโดยผู้ใช้รายอื่นแล้ว</span><span class="sxs-lookup"><span data-stu-id="a156a-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="a156a-115">ถ้าเป็นกรณีนี้ให้เอาอุปกรณ์ออกจากคอนโซล Azure Intune หรือยกเลิกการลงทะเบียนอุปกรณ์ด้วยตนเองก่อนที่จะลองอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="a156a-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="a156a-116">อุปกรณ์คือ Windows 10 Home</span><span class="sxs-lookup"><span data-stu-id="a156a-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="a156a-117">เฉพาะ Windows 10 Pro, การศึกษาและองค์กร Sku สามารถเข้าร่วมไดเรกทอรีที่ใช้งานอยู่ของ Azure</span><span class="sxs-lookup"><span data-stu-id="a156a-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="a156a-118">แหล่งข้อมูลเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="a156a-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="a156a-119">ใช้การ[แก้ปัญหาเว็บไซต์ Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัยและแก้ไขความล้มเหลวในการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="a156a-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="a156a-120">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="a156a-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="a156a-121">ตรวจทานเอกสารเหล่านี้สำหรับรายการข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและแก้ปัญหาสำหรับแต่ละ[คำแนะนำการแก้ไขปัญหา](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)และ[เอกสาร](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="a156a-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="a156a-122">[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="a156a-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
