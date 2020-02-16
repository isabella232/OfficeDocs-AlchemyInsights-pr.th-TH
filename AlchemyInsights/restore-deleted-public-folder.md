---
title: การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063766"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="a1e51-102">การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="a1e51-102">Restore a deleted public folder</span></span>

<span data-ttu-id="a1e51-103">**เมื่อต้องการคืนค่ารายการที่ถูกลบจากโฟลเดอร์สาธารณะ**:</span><span class="sxs-lookup"><span data-stu-id="a1e51-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="a1e51-104">ดู[คุณไม่สามารถกู้คืนรายการที่ถูกลบจากโฟลเดอร์สาธารณะที่ไม่ใช่จดหมายใน Outlook ๒๐๑๖](https://aka.ms/pfrec)</span><span class="sxs-lookup"><span data-stu-id="a1e51-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="a1e51-105">**เมื่อต้องการคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ (ชนิดใดก็ได้)**:</span><span class="sxs-lookup"><span data-stu-id="a1e51-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="a1e51-106">โปรดใช้คำสั่ง EXO PowerShell ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a1e51-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="a1e51-107">ไวยากรณ์:</span><span class="sxs-lookup"><span data-stu-id="a1e51-107">Syntax:</span></span>

    ><span data-ttu-id="a1e51-108">$pf = ได้รับ PublicFolder \ NON_IPM_SUBTREE DUMPSTER_ROOT-Recurse |? {$_. ชื่อ-eq "\<name_of_deleted_public_Folder"}; $Pf ตั้งค่า PublicFolder- \<เส้นทางเส้นทางที่จะคืนค่าโฟลเดอร์></span><span class="sxs-lookup"><span data-stu-id="a1e51-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="a1e51-109">ตัวอย่าง: คำสั่งต่อไปนี้จะคืนค่า Subfolder1 และวางภายใต้ \Parent1:</span><span class="sxs-lookup"><span data-stu-id="a1e51-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="a1e51-110">$pf = ได้รับ PublicFolder \ NON_IPM_SUBTREE DUMPSTER_ROOT-Recurse |? {$_. ชื่อ-eq "Subfolder1"}; $Pf ตั้งค่า PublicFolder-เส้นทาง \Parent1</span><span class="sxs-lookup"><span data-stu-id="a1e51-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="a1e51-111">ดู[ที่การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="a1e51-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
