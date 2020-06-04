---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intun
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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665851"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="abf4e-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intun</span><span class="sxs-lookup"><span data-stu-id="abf4e-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="abf4e-103">ตรวจสอบทรัพยากรที่แสดงด้านล่างเพื่อแก้ไขปัญหาของคุณตอนนี้</span><span class="sxs-lookup"><span data-stu-id="abf4e-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="abf4e-104">บางข้อความแสดงข้อผิดพลาดทั่วไปและขั้นตอนการแก้ปัญหา:</span><span class="sxs-lookup"><span data-stu-id="abf4e-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="abf4e-105">**ไม่สามารถติดตั้งซอฟต์แวร์ได้ 0x80cf4017:** ใบรับรองบัญชีของคุณหมดอายุแล้ว</span><span class="sxs-lookup"><span data-stu-id="abf4e-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="abf4e-106">ดาวน์โหลดแพคเกจซอฟต์แวร์ไคลเอ็นต์พีซีในคอนโซลผู้ดูแลระบบ Intun</span><span class="sxs-lookup"><span data-stu-id="abf4e-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="abf4e-107">อ่านเอกสารนี้สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="abf4e-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="abf4e-108">**รหัสข้อผิดพลาด 0x801c0003:** ข้อผิดพลาดสามารถเกิดขึ้นได้ในสถานการณ์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="abf4e-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="abf4e-109">ผู้ใช้มีอุปกรณ์ที่ลงทะเบียนมากกว่าขีดจํากัดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="abf4e-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="abf4e-110">ตรวจสอบเอกสารเหล่านี้เพื่อ[นําอุปกรณ์ออก](https://docs.microsoft.com/intune/devices-wipe)หรือ[เปลี่ยนขีดจํากัดของอุปกรณ์](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="abf4e-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="abf4e-111">"ผู้ใช้อาจเข้าร่วมอุปกรณ์ไปยังโฆษณา Azure" ถูกตั้งค่าเป็น "ไม่มี"</span><span class="sxs-lookup"><span data-stu-id="abf4e-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="abf4e-112">ตั้งค่าเป็นผู้ใช้ทั้งหมดหรือเลือก</span><span class="sxs-lookup"><span data-stu-id="abf4e-112">Set it to all or select users.</span></span> <span data-ttu-id="abf4e-113">อ่าน[เอกสารนี้](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="abf4e-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="abf4e-114">อุปกรณ์ถูกลงทะเบียนโดยผู้ใช้อื่นแล้ว</span><span class="sxs-lookup"><span data-stu-id="abf4e-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="abf4e-115">ถ้าเป็นกรณีนี้ ให้เอาอุปกรณ์ออกจากคอนโซล Azure Intunen หรือ unenroll อุปกรณ์ด้วยตนเองก่อนที่จะลองอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="abf4e-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="abf4e-116">อุปกรณ์เป็น Windows 10 หน้าแรก</span><span class="sxs-lookup"><span data-stu-id="abf4e-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="abf4e-117">เฉพาะ Windows 10 Pro, การศึกษาและองค์กร SKU เท่านั้นที่สามารถเข้าร่วมไดเรกทอรีที่ใช้งานอยู่ของ Azure</span><span class="sxs-lookup"><span data-stu-id="abf4e-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="abf4e-118">ทรัพยากรเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="abf4e-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="abf4e-119">ใช้[Intunเน เว็บไซต์การแก้ไขปัญหา](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัย และแก้ไขปัญหาความล้มเหลวในการลงทะเบียนทั่วไป</span><span class="sxs-lookup"><span data-stu-id="abf4e-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="abf4e-120">ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/intune/help-desk-operators)สําหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="abf4e-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="abf4e-121">ตรวจทานเอกสารเหล่านี้สําหรับรายการข้อผิดพลาดทั่วไปที่ป้องกันไม่ให้การลงทะเบียนและการแก้ปัญหาให้กับแต่ละ:[การแก้ไขปัญหาและการแก้ไขปัญหา](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)[เอกสาร](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="abf4e-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="abf4e-122">[เรียนรู้วิธีลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intun](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="abf4e-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
