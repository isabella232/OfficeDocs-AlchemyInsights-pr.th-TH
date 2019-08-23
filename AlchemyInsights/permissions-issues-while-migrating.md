---
title: การตัดสินค้าจากคลังสิทธิ์ขณะกำลังโยกย้าย
ms.author: kirks
author: Techwriter40
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 50f98fad1c4e37af1e8dacb76e0af1addafe0dc4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554927"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="1487e-102">ซิงโครไนส์ส่วนกำหนดค่าผู้ใช้และรูปถ่าย</span><span class="sxs-lookup"><span data-stu-id="1487e-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="1487e-103">**การซิงโครไนส์โพรไฟล์ภาพถ่าย**- ผู้ใช้อาจสังเกตเห็นว่า ภาพถ่ายโปรไฟล์ของพวกเขาจะไม่ซิงโครไนส์กับ SharePoint ได้</span><span class="sxs-lookup"><span data-stu-id="1487e-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="1487e-104">หรือ พวกเขาอาจพยายามจะปรับปรุงรูปถ่ายโปรไฟล์ของพวกเขา และรูปถ่ายยังคงปรากฏเป็นรูปถ่ายเก่า</span><span class="sxs-lookup"><span data-stu-id="1487e-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="1487e-105">เพื่อให้แน่ใจว่า โพรไฟล์รูปถ่ายแสดงตามที่คาดไว้ ผู้ใช้จะต้องเริ่มการซิงค์ภาพถ่าย</span><span class="sxs-lookup"><span data-stu-id="1487e-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="1487e-106">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับขั้นตอนการซิงโครไนส์ photo ดู[ข้อมูลเกี่ยวกับการซิงโครไนซ์รูปภาพในโปรไฟล์ใน Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="1487e-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="1487e-107">**ซิงโครไนส์โพรไฟล์**- เวลาที่ต้องดำเนินการซิงโครไนส์ของส่วนกำหนดค่าขึ้นอยู่กับจำนวนของงานนำเข้าโฆษณาที่มีการเปลี่ยนแปลง (งาน) กระบวนการ</span><span class="sxs-lookup"><span data-stu-id="1487e-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="1487e-108">ถ้ามีการเปลี่ยนแปลงมาก งานตัวจับเวลาได้จำนวนมากทำงานที่ต้องทำ และจะใช้เวลานานสำหรับการเปลี่ยนแปลงจะสะท้อนให้เห็นในโปรไฟล์ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="1487e-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="1487e-109">ถ้างานตัวจับเวลามีไดรฟ์ข้อมูลขนาดเล็กของงานการดำเนินการ การเปลี่ยนแปลงจะมีผลในโปรไฟล์ผู้ใช้ได้รวดเร็วมาก</span><span class="sxs-lookup"><span data-stu-id="1487e-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="1487e-110">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับขั้นตอนการซิงโครไนส์โพรไฟล์ ดู[ข้อมูลเกี่ยวกับการซิงโครไนส์ส่วนกำหนดค่าผู้ใช้ใน SharePoint แบบออนไลน์](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="1487e-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="1487e-111">การ**ปรับปรุงโปรไฟล์ใน Office Delve** - ผู้ใช้ Delve สามารถจัดการส่วนกำหนดค่าใน Office 365 ของพวกเขาได้</span><span class="sxs-lookup"><span data-stu-id="1487e-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="1487e-112">สำหรับข้อมูลเพิ่มเติม ดู[มุมมองและปรับปรุงส่วนกำหนดค่าของคุณใน Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)</span><span class="sxs-lookup"><span data-stu-id="1487e-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

