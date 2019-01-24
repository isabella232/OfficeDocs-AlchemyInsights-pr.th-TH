---
title: แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493543"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="25cfd-102">แก้ไขปัญหาเกี่ยวกับการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="25cfd-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="25cfd-103">ตรวจทานทรัพยากรแสดงรายการด้านล่างเพื่อแก้ไขปัญหาของคุณเดี๋ยวนี้</span><span class="sxs-lookup"><span data-stu-id="25cfd-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="25cfd-104">ข้อผิดพลาดทั่วไปบางอย่างและขั้นตอนการแก้ปัญหา:</span><span class="sxs-lookup"><span data-stu-id="25cfd-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="25cfd-p101">**ไม่สามารถติดตั้งซอฟต์แวร์ 0x80cf4017:** ใบรับรองบัญชีของคุณหมดอายุแล้ว ดาวน์โหลดแพคเกจซอฟต์แวร์ไคลเอนต์พีซีในคอนโซล Admin Intune อีกครั้ง ตรวจทานเอกสารนี้สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="25cfd-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="25cfd-108">**รหัสข้อผิดพลาด 0x801c0003:** ข้อผิดพลาดอาจเกิดขึ้นได้ในสถานการณ์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="25cfd-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="25cfd-p102">ผู้ใช้มีอุปกรณ์เพิ่มเติมที่ลงทะเบียนไว้เกินขีดจำกัดของอุปกรณ์ ตรวจทานเอกสารเหล่านี้เมื่อต้องการ[เอาอุปกรณ์ออก](https://docs.microsoft.com/en-us/intune/devices-wipe)หรือ[เปลี่ยนแปลงขีดจำกัดของอุปกรณ์](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="25cfd-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="25cfd-p103">"ผู้ใช้อาจเข้าร่วมอุปกรณ์เพื่อโฆษณา Azure" ถูกตั้งค่าเป็น "ไม่มี" ตั้งค่าทั้งหมด หรือเลือกผู้ใช้ ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings)สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="25cfd-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="25cfd-p104">อุปกรณ์มีการลงทะเบียนแล้ว โดยผู้ใช้อื่น ถ้าเป็นกรณีนี้ เอาอุปกรณ์ออกจากคอนโซล Azure Intune หรืออุปกรณ์ที่ unenroll ด้วยตนเองก่อนที่จะลองอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="25cfd-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="25cfd-p105">อุปกรณ์ดังกล่าว Windows 10 หน้าแรก เฉพาะ Windows 10 Pro การศึกษา และองค์กร Sku สามารถรวมไดเรกทอรีที่ใช้งานอยู่ของ Azure</span><span class="sxs-lookup"><span data-stu-id="25cfd-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="25cfd-118">ทรัพยากรเพิ่มเติมเพื่อช่วยแก้ไขปัญหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="25cfd-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="25cfd-p106">ใช้[ไซต์การแก้ไขปัญหาเบื้องต้น Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)เพื่อวินิจฉัย และแก้ปัญหาความล้มเหลวทั่วไปในการลงทะเบียน ตรวจทาน[เอกสารนี้](https://docs.microsoft.com/en-us/intune/help-desk-operators)สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="25cfd-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="25cfd-121">ตรวจทานเอกสารเหล่านี้สำหรับรายการของข้อผิดพลาดทั่วไปที่ป้องกันการลงทะเบียนและวิธีแก้ปัญหาแต่ละ:[คำแนะนำในการแก้ไขปัญหา](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)และการ[แก้ไขปัญหาเอกสาร](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="25cfd-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="25cfd-122">[เรียนรู้วิธีการลงทะเบียนอุปกรณ์ Windows ใน Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="25cfd-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

