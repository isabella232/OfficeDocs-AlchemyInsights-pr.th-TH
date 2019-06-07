---
title: ไม่สามารถลบสินค้าใน SharePoint หรือ OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 82a19c8ea218834b71901e95747da0c99243893e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757943"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="c7ba1-102">ไม่สามารถลบรายการ</span><span class="sxs-lookup"><span data-stu-id="c7ba1-102">Unable to delete items</span></span>

<span data-ttu-id="c7ba1-103">มีปัญหาการลบรายการหรือไม่</span><span class="sxs-lookup"><span data-stu-id="c7ba1-103">Having issues deleting items?</span></span>

- <span data-ttu-id="c7ba1-104">เสมอให้แน่ใจว่า คุณมี[สิทธิ์ที่เหมาะสม](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)เพื่อลบรายการ หรือมีความพยายามของ[ผู้ดูแลชุดเก็บรวบรวมไซต์](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)เอารายการนี้ออก</span><span class="sxs-lookup"><span data-stu-id="c7ba1-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="c7ba1-105">ให้แน่ใจว่า ไม่มีการตั้งค่า[นโยบายการเก็บข้อมูล](https://docs.microsoft.com/office365/securitycompliance/retention-policies)บนสินค้า</span><span class="sxs-lookup"><span data-stu-id="c7ba1-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="c7ba1-106">ให้แน่ใจว่า สินค้าจะไม่[ถูกเช็คเอาท์](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)ไปยังผู้ใช้อื่น</span><span class="sxs-lookup"><span data-stu-id="c7ba1-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="c7ba1-107">ในตอนท้าย ผู้ดูแลระบบสามารถใช้[รูปแบบของ SharePoint และวิธีปฏิบัติ](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)(PnP) ซึ่งประกอบด้วยไลบรารีของ PowerShell คำสั่งที่อนุญาตให้คุณทำการดำเนินการจัดการที่ซับซ้อนเช่น บังคับให้ลบรายการ stubborn</span><span class="sxs-lookup"><span data-stu-id="c7ba1-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="c7ba1-108">ลบไฟล์ PNP</span><span class="sxs-lookup"><span data-stu-id="c7ba1-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="c7ba1-109">เอาโฟลเดอร์ PNP</span><span class="sxs-lookup"><span data-stu-id="c7ba1-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="c7ba1-110">ลบสินค้าในรายการ PNP</span><span class="sxs-lookup"><span data-stu-id="c7ba1-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="c7ba1-111">เอารายการ PNP</span><span class="sxs-lookup"><span data-stu-id="c7ba1-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="c7ba1-112">เอา PNP เขตข้อมูล (คอลัมน์)</span><span class="sxs-lookup"><span data-stu-id="c7ba1-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)