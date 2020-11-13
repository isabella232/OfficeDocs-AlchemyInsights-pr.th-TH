---
title: ไม่สามารถลบรายการใน SharePoint หรือ OneDrive ได้
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019602"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="fc17d-102">ไม่สามารถลบรายการได้</span><span class="sxs-lookup"><span data-stu-id="fc17d-102">Unable to delete items</span></span>

- <span data-ttu-id="fc17d-103">นโยบายการเก็บข้อมูลอาจทำให้เกิดปัญหานี้ได้คุณจำเป็นต้องปิดใช้งานหรือไม่รวมการระงับที่เป็นสาเหตุของปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="fc17d-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="fc17d-104">หลังจากที่นโยบายการเก็บข้อมูลหรือการระงับถูกเอาออกอาจใช้เวลาถึง24ชั่วโมงเพื่อให้การเปลี่ยนแปลงมีผล</span><span class="sxs-lookup"><span data-stu-id="fc17d-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="fc17d-105">ตรวจสอบให้แน่ใจว่าไม่มีการตั้งค่า [นโยบายการเก็บข้อมูล](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) ในรายการ</span><span class="sxs-lookup"><span data-stu-id="fc17d-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="fc17d-106">ไซต์อาจเกินขีดจำกัดที่เก็บข้อมูลเพิ่ม [โควตาของไซต์](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) และลบรายการ</span><span class="sxs-lookup"><span data-stu-id="fc17d-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

- <span data-ttu-id="fc17d-107">ตรวจสอบให้แน่ใจว่ารายการไม่ได้ถูก [เช็คเอาท์](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ไปยังผู้ใช้อื่น</span><span class="sxs-lookup"><span data-stu-id="fc17d-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="fc17d-108">ในที่สุดผู้ดูแลระบบสามารถใช้ [รูปแบบของ SharePoint และวิธีปฏิบัติ](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ซึ่งมีไลบรารีของคำสั่ง PowerShell ที่ช่วยให้คุณสามารถดำเนินการการจัดการที่ซับซ้อนเช่นบังคับให้มีการลบรายการที่เป็นปาก</span><span class="sxs-lookup"><span data-stu-id="fc17d-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="fc17d-109">เอาไฟล์ PNP ออก</span><span class="sxs-lookup"><span data-stu-id="fc17d-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="fc17d-110">เอาโฟลเดอร์ PNP ออก</span><span class="sxs-lookup"><span data-stu-id="fc17d-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="fc17d-111">เอารายการ PNP ออก</span><span class="sxs-lookup"><span data-stu-id="fc17d-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="fc17d-112">เอารายการ PNP ออก</span><span class="sxs-lookup"><span data-stu-id="fc17d-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="fc17d-113">เอาเขตข้อมูล PNP (คอลัมน์) ออก</span><span class="sxs-lookup"><span data-stu-id="fc17d-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)