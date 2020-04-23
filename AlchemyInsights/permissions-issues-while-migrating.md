---
title: ปัญหาเกี่ยวกับสิทธิ์ขณะย้ายข้อมูล
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 077b7cf29ef6a40ef7f2aebef15e39a0f5df0fc3
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758989"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="e3fa9-102">การซิงโครไนซ์โปรไฟล์ผู้ใช้และรูปถ่าย</span><span class="sxs-lookup"><span data-stu-id="e3fa9-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="e3fa9-103">**การซิงโครไนส์ภาพถ่ายโปรไฟล์**- ผู้ใช้อาจสังเกตเห็นว่า รูปโปรไฟล์ของพวกเขาจะไม่ซิงโครไนส์กับ SharePoint</span><span class="sxs-lookup"><span data-stu-id="e3fa9-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="e3fa9-104">พวกเขาอาจพยายามอัพเดตรูปโปรไฟล์และรูปภาพยังคงปรากฏเป็นรูปภาพเก่า</span><span class="sxs-lookup"><span data-stu-id="e3fa9-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="e3fa9-105">ผู้ใช้จะต้องเริ่มต้นการซิงค์ภาพถ่าย</span><span class="sxs-lookup"><span data-stu-id="e3fa9-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="e3fa9-106">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับกระบวนการซิงโครไนส์ภาพถ่าย ให้ดู[ข้อมูลเกี่ยวกับการทําข้อมูลรูปภาพโปรไฟล์ใน Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)ให้ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="e3fa9-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="e3fa9-107">**ซิงโครไนส์ส่วนกําหนดค่า**- เวลาที่จําเป็นต้องทําข้อมูลส่วนกําหนดค่าให้ตรงกันขึ้นอยู่กับจํานวนของการเปลี่ยนแปลง (งาน) งานการนําเข้าโฆษณามีการประมวลผล</span><span class="sxs-lookup"><span data-stu-id="e3fa9-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="e3fa9-108">ถ้ามีการเปลี่ยนแปลงมากมาย งานตัวจับเวลามีงานต้องทํามากมาย และจะใช้เวลานานกว่าสําหรับการเปลี่ยนแปลงที่จะปรากฏในโปรแกรมประยุกต์โปรไฟล์ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="e3fa9-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="e3fa9-109">ถ้างานตัวจับเวลามีปริมาณการทํางานขนาดเล็กที่ต้องทําการเปลี่ยนแปลงจะปรากฏในการประยุกต์ใช้รายละเอียดผู้ใช้ได้เร็วขึ้นมาก</span><span class="sxs-lookup"><span data-stu-id="e3fa9-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="e3fa9-110">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับกระบวนการซิงโครไนส์ส่วนกําหนดค่า ให้ดู[ข้อมูลเกี่ยวกับการซิงโครไนส์ส่วนกําหนดค่าผู้ใช้ใน SharePoint แบบออนไลน์](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="e3fa9-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="e3fa9-111">**ปรับปรุงโปรไฟล์ใน Office Delve** - ผู้ใช้ Delve สามารถจัดการโปรไฟล์ของ Microsoft 365 ได้</span><span class="sxs-lookup"><span data-stu-id="e3fa9-111">**Update Profile in Office Delve** - Delve users can manage their Microsoft 365 Profile.</span></span> <span data-ttu-id="e3fa9-112">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การดูและอัปเดตโปรไฟล์ของคุณใน Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)</span><span class="sxs-lookup"><span data-stu-id="e3fa9-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

