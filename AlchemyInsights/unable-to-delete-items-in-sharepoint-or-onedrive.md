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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511995"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="4d5b3-102">ไม่สามารถลบรายการ</span><span class="sxs-lookup"><span data-stu-id="4d5b3-102">Unable to delete items</span></span>

<span data-ttu-id="4d5b3-103">นโยบายการเก็บข้อมูลอาจทําให้เกิดปัญหานี้ คุณจําเป็นต้องปิดใช้งานหรือยกเว้นการหยุดที่เกี่ยวข้องที่เป็นสาเหตุของปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="4d5b3-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="4d5b3-104">หลังจากลบนโยบายการเก็บข้อมูลหรือการเก็บรักษาแล้ว อาจใช้เวลาถึง 24 ชั่วโมงเพื่อให้การเปลี่ยนแปลงมีผล</span><span class="sxs-lookup"><span data-stu-id="4d5b3-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="4d5b3-105">ตรวจสอบให้แน่ใจว่าไม่มีการตั้งค่า[นโยบายการเก็บข้อมูล](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)บนรายการ</span><span class="sxs-lookup"><span data-stu-id="4d5b3-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="4d5b3-106">ไซต์อาจเกินขีดจํากัดของพื้นที่เก็บข้อมูล ให้เพิ่ม[โควต้าไซต์](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)และลบรายการนั้น</span><span class="sxs-lookup"><span data-stu-id="4d5b3-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="4d5b3-107">ตรวจสอบให้แน่ใจว่ารายการไม่ได้ถูก[เช็คเอาท์](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)ไปยังผู้ใช้อื่น</span><span class="sxs-lookup"><span data-stu-id="4d5b3-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="4d5b3-108">สุดท้าย ผู้ดูแลระบบสามารถใช้[รูปแบบและวิธีปฏิบัติของ SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ซึ่งประกอบด้วยไลบรารีของคําสั่ง PowerShell ที่อนุญาตให้คุณดําเนินการจัดการที่ซับซ้อนเช่นบังคับให้ลบรายการปากแข็ง</span><span class="sxs-lookup"><span data-stu-id="4d5b3-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="4d5b3-109">เอาแฟ้ม PNP ออก</span><span class="sxs-lookup"><span data-stu-id="4d5b3-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="4d5b3-110">ลบโฟลเดอร์ PNP</span><span class="sxs-lookup"><span data-stu-id="4d5b3-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="4d5b3-111">เอารายการ PNP ออก</span><span class="sxs-lookup"><span data-stu-id="4d5b3-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="4d5b3-112">ลบรายการ PNP</span><span class="sxs-lookup"><span data-stu-id="4d5b3-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="4d5b3-113">เอาเขตข้อมูล PNP ออก (คอลัมน์)</span><span class="sxs-lookup"><span data-stu-id="4d5b3-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)