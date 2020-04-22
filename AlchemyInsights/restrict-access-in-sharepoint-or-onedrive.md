---
title: จํากัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715903"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="26f29-102">จํากัดการเข้าถึงใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="26f29-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="26f29-103">ใน SharePoint และ OneDrive คุณสามารถจํากัดการเข้าถึงรายการต่างๆ เช่น ไฟล์ โฟลเดอร์ และรายการโดยการอนุญาตให้เข้าถึงเฉพาะกลุ่มหรือบุคคลที่คุณต้องการให้เข้าถึงเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="26f29-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="26f29-104">โดยค่าเริ่มต้น สิทธิ์ใน SharePoint จะสืบทอดจากสูงกว่าในลําดับชั้น</span><span class="sxs-lookup"><span data-stu-id="26f29-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="26f29-105">แฟ้มสืบทอดสิทธิ์จากโฟลเดอร์ ซึ่งสืบทอดสิทธิ์จากไลบรารี ซึ่งสืบทอดสิทธิ์จากไซต์</span><span class="sxs-lookup"><span data-stu-id="26f29-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="26f29-106">คุณสามารถใช้ร่วมกันในระดับที่สูงกว่า (เช่น โดยการแชร์ทั้งไซต์) แล้วหยุดการสืบทอดถ้าคุณไม่ต้องการใช้รายการทั้งหมดบนไซต์ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="26f29-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="26f29-107">อย่างไรก็ตามเราไม่แนะนําเพราะจะทําให้การรักษาสิทธิ์ที่ซับซ้อนมากขึ้นและสับสนในอนาคต</span><span class="sxs-lookup"><span data-stu-id="26f29-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="26f29-108">นี่คือสิ่งที่คุณสามารถทําได้แทน:</span><span class="sxs-lookup"><span data-stu-id="26f29-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="26f29-109">ตัวอย่างเช่น ถ้าคุณต้องการใช้เนื้อหาทั้งหมดของโฟลเดอร์ร่วมกัน ยกเว้นแฟ้มหนึ่งในโฟลเดอร์ นั้น ให้ย้ายแฟ้มนั้นไปยังตําแหน่งใหม่ที่ไม่ได้แชร์</span><span class="sxs-lookup"><span data-stu-id="26f29-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="26f29-110">ถ้าคุณมีโฟลเดอร์ย่อยสองโฟลเดอร์ และคุณต้องการแชร์โฟลเดอร์ย่อยหนึ่งโฟลเดอร์กับกลุ่ม A และ B และอนุญาตให้เฉพาะกลุ่ม A และ B เข้าถึงโฟลเดอร์ย่อยที่สองให้แชร์โฟลเดอร์หลักกับกลุ่ม A และเพิ่มกลุ่ม B ลงในโฟลเดอร์ย่อยแรก</span><span class="sxs-lookup"><span data-stu-id="26f29-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="26f29-111">หยุดการใช้แฟ้มหรือโฟลเดอร์ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="26f29-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

