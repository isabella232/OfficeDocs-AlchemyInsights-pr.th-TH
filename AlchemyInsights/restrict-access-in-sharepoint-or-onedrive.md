---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551470"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="438ee-102">จำกัดการเข้าถึงใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="438ee-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="438ee-103">ใน SharePoint และ OneDrive คุณจำกัดการเข้าถึงรายการต่างๆเช่นแฟ้มโฟลเดอร์และรายการโดยให้สิทธิ์การเข้าถึงเฉพาะกลุ่มหรือบุคคลที่คุณต้องการเข้าถึงเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="438ee-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="438ee-104">โดยค่าเริ่มต้นสิทธิ์ใน SharePoint จะได้รับการสืบทอดมาจากสูงขึ้นในลำดับชั้น</span><span class="sxs-lookup"><span data-stu-id="438ee-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="438ee-105">ดังนั้นไฟล์ที่สืบทอดสิทธิ์จากโฟลเดอร์ซึ่งสืบทอดสิทธิ์จากไลบรารีซึ่งสืบทอดสิทธิ์จากเว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="438ee-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="438ee-106">คุณสามารถแชร์ในระดับที่สูงกว่า (เช่นการแชร์เว็บไซต์ทั้งหมด) แล้วหยุดการสืบทอดถ้าคุณไม่ต้องการแชร์รายการทั้งหมดบนไซต์</span><span class="sxs-lookup"><span data-stu-id="438ee-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="438ee-107">อย่างไรก็ตาม, เราไม่แนะนำนี้เพราะมันทำให้การรักษาสิทธิ์ที่ซับซ้อนมากขึ้นและสับสนในอนาคต.</span><span class="sxs-lookup"><span data-stu-id="438ee-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="438ee-108">นี่คือสิ่งที่คุณสามารถทำได้แทน:</span><span class="sxs-lookup"><span data-stu-id="438ee-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="438ee-109">ตัวอย่างเช่นถ้าคุณต้องการใช้เนื้อหาทั้งหมดของโฟลเดอร์ร่วมกันยกเว้นแฟ้มเดียวในนั้นให้ย้ายแฟ้มนั้นไปยังตำแหน่งใหม่ที่ไม่ได้ใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="438ee-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="438ee-110">ถ้าคุณมีสองโฟลเดอร์ย่อยในโฟลเดอร์และคุณต้องการแชร์โฟลเดอร์ย่อยหนึ่งกับกลุ่ม A และ B และอนุญาตเฉพาะกลุ่มการเข้าถึงโฟลเดอร์ย่อยที่สองให้ใช้โฟลเดอร์หลักร่วมกับกลุ่ม A และเพิ่มกลุ่ม B ลงในโฟลเดอร์ย่อยแรก</span><span class="sxs-lookup"><span data-stu-id="438ee-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="438ee-111">หยุดการใช้แฟ้มหรือโฟลเดอร์ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="438ee-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

