---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720701"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="308d9-102">จำกัดการเข้าถึงใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="308d9-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="308d9-103">ใน SharePoint และ OneDrive คุณจำกัดการเข้าถึงรายการเช่นไฟล์โฟลเดอร์และรายการโดยให้สิทธิ์การเข้าถึงแก่กลุ่มหรือบุคคลที่คุณต้องการเข้าถึงเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="308d9-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="308d9-104">ตามค่าเริ่มต้นสิทธิ์ใน SharePoint จะถูกสืบทอดมาจากที่สูงขึ้นในลำดับชั้น</span><span class="sxs-lookup"><span data-stu-id="308d9-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="308d9-105">ดังนั้นไฟล์จะสืบทอดสิทธิ์จากโฟลเดอร์ซึ่งสืบทอดสิทธิ์จากไลบรารีซึ่งสืบทอดสิทธิ์จากไซต์</span><span class="sxs-lookup"><span data-stu-id="308d9-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="308d9-106">คุณสามารถแชร์ได้ในระดับที่สูงขึ้น (เช่นโดยการแชร์ทั้งไซต์) แล้วแบ่งการสืบทอดถ้าคุณไม่ต้องการแชร์รายการทั้งหมดบนไซต์</span><span class="sxs-lookup"><span data-stu-id="308d9-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="308d9-107">อย่างไรก็ตามเราไม่แนะนำสิ่งนี้เนื่องจากจะทำให้สิทธิ์การใช้งานที่ซับซ้อนมากขึ้นและสับสนในอนาคต</span><span class="sxs-lookup"><span data-stu-id="308d9-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="308d9-108">ต่อไปนี้คือสิ่งที่คุณสามารถทำได้แทน:</span><span class="sxs-lookup"><span data-stu-id="308d9-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="308d9-109">ตัวอย่างเช่นถ้าคุณต้องการแชร์เนื้อหาของโฟลเดอร์ทั้งหมดยกเว้นไฟล์หนึ่งในไฟล์นั้นให้ย้ายไฟล์นั้นไปยังตำแหน่งที่ตั้งใหม่ที่ไม่ได้แชร์</span><span class="sxs-lookup"><span data-stu-id="308d9-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="308d9-110">ถ้าคุณมีโฟลเดอร์ย่อยสองโฟลเดอร์ในโฟลเดอร์และคุณต้องการแชร์โฟลเดอร์ย่อยหนึ่งโฟลเดอร์กับกลุ่ม A และ B และอนุญาตเฉพาะกลุ่มการเข้าถึงโฟลเดอร์ย่อยที่สองให้แชร์โฟลเดอร์แม่กับกลุ่ม A และเพิ่มกลุ่ม B ไปยังโฟลเดอร์ย่อยแรก</span><span class="sxs-lookup"><span data-stu-id="308d9-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="308d9-111">หยุดการแชร์ไฟล์หรือโฟลเดอร์ </span><span class="sxs-lookup"><span data-stu-id="308d9-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

