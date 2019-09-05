---
title: ปัญหาเกี่ยวกับสิทธิ์ขณะโยกย้าย
ms.author: pebaum
author: Techwriter40
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 33e605ff3019f52bbd0be876d485ff389b260a44
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752642"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="210eb-102">โปรไฟล์ผู้ใช้และการซิงโครไนซ์รูปภาพ</span><span class="sxs-lookup"><span data-stu-id="210eb-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="210eb-103">**โปรไฟล์การซิงโครไนส์รูปภาพ**-ผู้ใช้อาจสังเกตเห็นว่ารูปโปรไฟล์ของพวกเขาจะไม่ซิงโครไนส์กับ SharePoint</span><span class="sxs-lookup"><span data-stu-id="210eb-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="210eb-104">หรือพวกเขาอาจพยายามที่จะปรับปรุงรูปโปรไฟล์ของพวกเขาและรูปภาพยังคงปรากฏเป็นภาพเก่า</span><span class="sxs-lookup"><span data-stu-id="210eb-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="210eb-105">เพื่อให้แน่ใจว่ารูปโปรไฟล์แสดงตามที่คาดไว้ผู้ใช้จะต้องเริ่มต้นการซิงค์รูปภาพ</span><span class="sxs-lookup"><span data-stu-id="210eb-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="210eb-106">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับกระบวนการซิงโครไนส์รูปภาพโปรดดู[ข้อมูลเกี่ยวกับการซิงโครไนส์รูปโปรไฟล์ใน Office ๓๖๕](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="210eb-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="210eb-107">การ**ซิงโครไนส์โปรไฟล์**-เวลาที่จำเป็นในการทำข้อมูลให้ตรงกันของโปรไฟล์เสร็จสมบูรณ์ขึ้นอยู่กับจำนวนการเปลี่ยนแปลง (ทำงาน) ที่งานนำเข้าโฆษณามีการประมวลผล</span><span class="sxs-lookup"><span data-stu-id="210eb-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="210eb-108">หากมีการเปลี่ยนแปลงหลายรายการงานตัวจับเวลามีจำนวนมากของงานที่ต้องทำและจะใช้เวลานานขึ้นสำหรับการเปลี่ยนแปลงที่จะสะท้อนให้เห็นในโปรแกรมประยุกต์ส่วนกำหนดค่าผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="210eb-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="210eb-109">ถ้างานตัวจับเวลามีปริมาณขนาดเล็กของงานที่จะทำการเปลี่ยนแปลงจะปรากฏในโปรแกรมประยุกต์ส่วนกำหนดค่าผู้ใช้ได้เร็วขึ้นมาก</span><span class="sxs-lookup"><span data-stu-id="210eb-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="210eb-110">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับกระบวนการซิงโครไนส์โพรไฟล์ดู[ข้อมูลเกี่ยวกับการซิงโครไนส์ส่วนกำหนดค่าผู้ใช้ใน SharePoint แบบออนไลน์](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="210eb-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="210eb-111">**ปรับปรุงส่วนกำหนดค่าในผู้ใช้ Office delve** -delve สามารถจัดการกับ Office ๓๖๕โปรไฟล์ของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="210eb-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="210eb-112">สำหรับข้อมูลเพิ่มเติมโปรดดูที่[การดูและปรับปรุงส่วนกำหนดค่าของคุณใน Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)</span><span class="sxs-lookup"><span data-stu-id="210eb-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

