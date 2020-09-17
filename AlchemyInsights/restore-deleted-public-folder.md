---
title: การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774550"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="00b4a-102">การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="00b4a-102">Restore a deleted public folder</span></span>

<span data-ttu-id="00b4a-103">**เมื่อต้องการคืนค่ารายการที่ถูกลบจากโฟลเดอร์สาธารณะให้ใช้วิธีต่อไป**นี้</span><span class="sxs-lookup"><span data-stu-id="00b4a-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="00b4a-104">ให้ดู[ที่คุณไม่สามารถกู้คืนรายการที่ถูกลบจากโฟลเดอร์สาธารณะที่ไม่ใช่อีเมลใน Outlook ๒๐๑๖](https://aka.ms/pfrec)</span><span class="sxs-lookup"><span data-stu-id="00b4a-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="00b4a-105">**เมื่อต้องการคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ (ชนิดใดก็ตาม)**:</span><span class="sxs-lookup"><span data-stu-id="00b4a-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="00b4a-106">โปรดใช้คำสั่ง EXO PowerShell ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="00b4a-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="00b4a-107">ไวยากรณ์ของ</span><span class="sxs-lookup"><span data-stu-id="00b4a-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="00b4a-108">ตัวอย่าง: คำสั่งต่อไปนี้จะคืนค่า Subfolder1 และวางภายใต้ \Parent1:</span><span class="sxs-lookup"><span data-stu-id="00b4a-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="00b4a-109">ให้ดู [ที่คืนค่าโฟลเดอร์สาธารณะที่ถูกลบ](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="00b4a-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
