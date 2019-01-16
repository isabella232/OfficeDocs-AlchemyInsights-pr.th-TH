---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28316788"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="ae830-102">จำกัดการเข้าถึงใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="ae830-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="ae830-p101">ใน SharePoint และ OneDrive คุณจำกัดการเข้าถึงรายการอย่างเช่นไฟล์ โฟลเดอร์ และรายการ โดยให้การเข้าถึงเฉพาะกลุ่มหรือบุคคลที่คุณต้องการให้มีการเข้าถึง โดยค่าเริ่มต้น สิทธิ์ใน SharePoint จะถูกสืบทอดจากค่าที่สูงกว่าในลำดับชั้น ดังนั้น แฟ้มสืบทอดสิทธิ์จากโฟลเดอร์ ซึ่งสืบทอดสิทธิ์จากไลบรารี ที่สืบทอดสิทธิ์จากไซต์</span><span class="sxs-lookup"><span data-stu-id="ae830-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="ae830-p102">คุณสามารถใช้ร่วมกันในระดับสูงกว่า (เช่น โดยการใช้ร่วมกันทั้งไซต์) และตัดการสืบทอดจากนั้น ถ้าคุณไม่ต้องการสินค้าทั้งหมดบนไซต์ที่ใช้ร่วมกันได้ อย่างไรก็ตาม เราไม่แนะนำเช่นนี้เนื่องจากจะทำให้การรักษาสิทธิ์ที่ซับซ้อน และสับสนในอนาคต ต่อไปนี้คือสิ่งที่คุณไม่สามารถทำแทน:</span><span class="sxs-lookup"><span data-stu-id="ae830-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="ae830-109">ถ้า ตัวอย่างเช่น คุณต้องการเนื้อหาทั้งหมดยกเว้นสำหรับแฟ้มหนึ่งแฟ้มในโฟลเดอร์ที่ใช้ร่วมกัน ย้ายแฟ้มนั้นไปยังตำแหน่งใหม่ที่ไม่ได้ใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="ae830-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="ae830-110">ถ้าคุณมีโฟลเดอร์ย่อยที่สองในโฟลเดอร์ และคุณต้องการใช้ร่วมกันโฟลเดอร์ย่อยหนึ่งกับกลุ่ม A และ B และอนุญาตให้เฉพาะกลุ่ม A เข้าถึงโฟลเดอร์ย่อยที่สอง ใช้ร่วมกันโฟลเดอร์หลักกับกลุ่ม A และเพิ่มกลุ่ม B ถึงโฟลเดอร์ย่อยแรก</span><span class="sxs-lookup"><span data-stu-id="ae830-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="ae830-111">หยุดการใช้แฟ้มหรือโฟลเดอร์ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="ae830-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

