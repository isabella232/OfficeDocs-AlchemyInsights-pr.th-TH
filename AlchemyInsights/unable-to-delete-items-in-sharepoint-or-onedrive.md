---
title: ไม่สามารถลบรายการใน SharePoint หรือ OneDrive ได้
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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571290"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="8ad3e-102">ไม่สามารถลบรายการ</span><span class="sxs-lookup"><span data-stu-id="8ad3e-102">Unable to delete items</span></span>

<span data-ttu-id="8ad3e-103">นโยบายการเก็บข้อมูลอาจทำให้เกิดปัญหานี้คุณจำเป็นต้องปิดใช้งานหรือไม่รวมการระงับที่เกี่ยวข้องกับสาเหตุนี้</span><span class="sxs-lookup"><span data-stu-id="8ad3e-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="8ad3e-104">หลังจากที่นโยบายการเก็บข้อมูลหรือระงับไว้จะถูกเอาออกอาจใช้เวลาถึง24ชั่วโมงสำหรับการเปลี่ยนแปลงจะมีผล</span><span class="sxs-lookup"><span data-stu-id="8ad3e-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="8ad3e-105">ตรวจสอบให้แน่ใจว่าไม่มีการตั้งค่า[นโยบายการเก็บข้อมูล](https://docs.microsoft.com/office365/securitycompliance/retention-policies)บนสินค้า</span><span class="sxs-lookup"><span data-stu-id="8ad3e-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="8ad3e-106">ไซต์อาจเกินขีดจำกัดการเก็บข้อมูลเพิ่ม[โควตาของไซต์](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)และลบรายการ</span><span class="sxs-lookup"><span data-stu-id="8ad3e-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="8ad3e-107">ตรวจสอบให้แน่ใจว่าสินค้าไม่ได้ถูก[เช็คเอาท์](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)ไปยังผู้ใช้อื่น</span><span class="sxs-lookup"><span data-stu-id="8ad3e-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="8ad3e-108">ในที่สุดผู้ดูแลระบบสามารถใช้[รูปแบบของ SharePoint และวิธีปฏิบัติ](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)(PnP) ซึ่งประกอบด้วยไลบรารีของคำสั่ง PowerShell ที่ช่วยให้คุณสามารถทำการดำเนินการจัดการที่ซับซ้อนเช่นบังคับการลบรายการที่เป็นปาก</span><span class="sxs-lookup"><span data-stu-id="8ad3e-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="8ad3e-109">เอาแฟ้ม PNP</span><span class="sxs-lookup"><span data-stu-id="8ad3e-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="8ad3e-110">เอาโฟลเดอร์ PNP ออก</span><span class="sxs-lookup"><span data-stu-id="8ad3e-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="8ad3e-111">เอารายการ PNP</span><span class="sxs-lookup"><span data-stu-id="8ad3e-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="8ad3e-112">เอารายการ PNP</span><span class="sxs-lookup"><span data-stu-id="8ad3e-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="8ad3e-113">เอาเขตข้อมูล PNP (คอลัมน์)</span><span class="sxs-lookup"><span data-stu-id="8ad3e-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)