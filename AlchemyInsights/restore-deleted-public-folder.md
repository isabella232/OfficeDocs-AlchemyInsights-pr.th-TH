---
title: คืนค่าโฟลเดอร์สาธารณะที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809458"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="5d934-102">คืนค่าโฟลเดอร์สาธารณะที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="5d934-102">Restore a deleted public folder</span></span>

<span data-ttu-id="5d934-103">**เมื่อต้องการคืนค่ารายการที่ถูกลบจากโฟลเดอร์สาธารณะ**:</span><span class="sxs-lookup"><span data-stu-id="5d934-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="5d934-104">ดู [คุณไม่สามารถกู้คืนรายการที่ถูกลบจากโฟลเดอร์สาธารณะที่ไม่ใช่จดหมายใน Outlook 2016](https://aka.ms/pfrec)ได้</span><span class="sxs-lookup"><span data-stu-id="5d934-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="5d934-105">**เมื่อต้องการคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ (ชนิดใดๆ)**:</span><span class="sxs-lookup"><span data-stu-id="5d934-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="5d934-106">โปรดใช้การสั่ง EXO PowerShell ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="5d934-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="5d934-107">ไวยากรณ์:</span><span class="sxs-lookup"><span data-stu-id="5d934-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="5d934-108">ตัวอย่าง: The following command will restore Subfolder1 and place it under \Parent1:</span><span class="sxs-lookup"><span data-stu-id="5d934-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="5d934-109">ดูรายละเอียด [เพิ่มเติมที่ คืนค่าโฟลเดอร์](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) สาธารณะที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="5d934-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
