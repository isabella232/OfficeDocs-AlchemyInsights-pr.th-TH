---
title: ไม่สามารถลบรายการใน SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049536"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="52ea4-102">ไม่สามารถลบรายการได้</span><span class="sxs-lookup"><span data-stu-id="52ea4-102">Unable to delete items</span></span>

<span data-ttu-id="52ea4-103">มีปัญหาในการลบรายการ SharePoint หรือไม่</span><span class="sxs-lookup"><span data-stu-id="52ea4-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="52ea4-104">โปรดตรวจสอบให้แน่ใจว่าคุณมี[สิทธิ์ที่เหมาะสม](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)เพื่อลบรายการหรือมี[ผู้ดูแลชุดเก็บรวบรวมไซต์](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)พยายามเอารายการออก</span><span class="sxs-lookup"><span data-stu-id="52ea4-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="52ea4-105">ตรวจสอบให้แน่ใจว่าไม่มีการตั้งค่า[นโยบายการเก็บข้อมูล](https://docs.microsoft.com/office365/securitycompliance/retention-policies)ในสินค้า</span><span class="sxs-lookup"><span data-stu-id="52ea4-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="52ea4-106">ตรวจสอบให้แน่ใจว่ารายการไม่ได้ถูก[เช็คเอาท์](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)ไปยังผู้ใช้อื่น</span><span class="sxs-lookup"><span data-stu-id="52ea4-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="52ea4-107">ในที่สุดผู้ดูแลระบบสามารถใช้[รูปแบบและวิธีปฏิบัติของ SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ซึ่งประกอบด้วยไลบรารีของคำสั่ง PowerShell ที่ช่วยให้คุณสามารถดำเนินการจัดการที่ซับซ้อนเช่นการบังคับให้ลบรายการที่ปากแข็ง</span><span class="sxs-lookup"><span data-stu-id="52ea4-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="52ea4-108">เอาแฟ้ม PNP ออก</span><span class="sxs-lookup"><span data-stu-id="52ea4-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="52ea4-109">ลบโฟลเดอร์ PNP</span><span class="sxs-lookup"><span data-stu-id="52ea4-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="52ea4-110">ลบรายการ PNP</span><span class="sxs-lookup"><span data-stu-id="52ea4-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="52ea4-111">ลบรายการ PNP</span><span class="sxs-lookup"><span data-stu-id="52ea4-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="52ea4-112">ลบฟิลด์ PNP (คอลัมน์)</span><span class="sxs-lookup"><span data-stu-id="52ea4-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)