---
title: ปัญหาสิทธิ์ขณะโยกย้าย
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 39b36a85319ccd71278571f3a3cbbc7cf0b9f0fa
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798071"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="c6d77-102">โปรไฟล์ผู้ใช้และการซิงโครไนซ์รูปถ่าย</span><span class="sxs-lookup"><span data-stu-id="c6d77-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="c6d77-103">การ**ซิงโครไนซ์รูปภาพโปรไฟล์**-ผู้ใช้อาจสังเกตเห็นว่ารูปโปรไฟล์ของพวกเขาไม่ได้ซิงโครไนซ์กับ SharePoint</span><span class="sxs-lookup"><span data-stu-id="c6d77-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="c6d77-104">หรือบุคคลเหล่านั้นอาจพยายามอัปเดตรูปภาพโพรไฟล์ของพวกเขาและรูปภาพยังคงปรากฏเป็นรูปถ่ายเก่า</span><span class="sxs-lookup"><span data-stu-id="c6d77-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="c6d77-105">เมื่อต้องการตรวจสอบให้แน่ใจว่ารูปโปรไฟล์แสดงตามที่คาดไว้ผู้ใช้จะต้องเริ่มการซิงค์รูปถ่าย</span><span class="sxs-lookup"><span data-stu-id="c6d77-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="c6d77-106">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับขั้นตอนการซิงโครไนซ์รูปภาพให้ดู [ข้อมูลเกี่ยวกับการซิงโครไนซ์รูปภาพโปรไฟล์ใน Microsoft ๓๖๕](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="c6d77-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="c6d77-107">การ**ซิงโครไนซ์โปรไฟล์**-เวลาที่จำเป็นในการทำให้การซิงโครไนซ์โปรไฟล์เสร็จสมบูรณ์ขึ้นอยู่กับจำนวนการเปลี่ยนแปลง (ทำงาน) งานนำเข้าของโฆษณาที่มีการประมวลผล</span><span class="sxs-lookup"><span data-stu-id="c6d77-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="c6d77-108">ถ้ามีการเปลี่ยนแปลงจำนวนมากงานตัวจับเวลาจะมีงานจำนวนมากที่ต้องทำและจะใช้เวลานานขึ้นสำหรับการเปลี่ยนแปลงที่จะปรากฏในแอปพลิเคชันโปรไฟล์ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="c6d77-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="c6d77-109">ถ้างานตัวจับเวลามีขนาดเล็กของงานที่ต้องการทำการเปลี่ยนแปลงจะปรากฏในแอปพลิเคชันโปรไฟล์ผู้ใช้ได้เร็วขึ้นมาก</span><span class="sxs-lookup"><span data-stu-id="c6d77-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="c6d77-110">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับขั้นตอนการซิงโครไนซ์โปรไฟล์ให้ดู [ข้อมูลเกี่ยวกับการซิงโครไนซ์โปรไฟล์ผู้ใช้ใน SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="c6d77-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="c6d77-111">**อัปเดตโปรไฟล์ใน Office delve** -delve ผู้ใช้สามารถจัดการโปรไฟล์ Microsoft ๓๖๕ของพวกเขาได้</span><span class="sxs-lookup"><span data-stu-id="c6d77-111">**Update Profile in Office Delve** - Delve users can manage their Microsoft 365 Profile.</span></span> <span data-ttu-id="c6d77-112">สำหรับข้อมูลเพิ่มเติมให้ดูที่[ดูและอัปเดตโปรไฟล์ของคุณใน Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)</span><span class="sxs-lookup"><span data-stu-id="c6d77-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

