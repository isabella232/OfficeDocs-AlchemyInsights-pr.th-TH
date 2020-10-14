---
title: ส่งเป็นโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมายใน EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/13/2020
ms.locfileid: "48462075"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="8f26f-102">โฟลเดอร์สาธารณะที่เปิดใช้งาน SendAs Mail</span><span class="sxs-lookup"><span data-stu-id="8f26f-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="8f26f-103">ตัวอย่างต่อไปนี้จะกำหนดสิทธิ์ "ส่งเป็น" สำหรับโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย NewPF1 ไปยังผู้ใช้ Jason</span><span class="sxs-lookup"><span data-stu-id="8f26f-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="8f26f-104">Add-RecipientPermission-ข้อมูลประจำตัว ' NewPF1 '-ทรัสตี "เจสัน"-AccessRights ' SendAs '</span><span class="sxs-lookup"><span data-stu-id="8f26f-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="8f26f-105">สำหรับรายละเอียดไวยากรณ์และข้อมูลพารามิเตอร์ให้ดู[ที่กำหนดสิทธิ์ "ส่งเป็น" หรือ "ส่งในนาม" สำหรับโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)</span><span class="sxs-lookup"><span data-stu-id="8f26f-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

