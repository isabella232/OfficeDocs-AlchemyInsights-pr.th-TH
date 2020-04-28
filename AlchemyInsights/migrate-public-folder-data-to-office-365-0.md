---
title: ย้ายข้อมูลโฟลเดอร์สาธารณะไปยัง Microsoft 365
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "639"
- "3500007"
ms.assetid: 6e536c7d-ab36-413e-9702-63e51adb3452
ms.openlocfilehash: ab54d84f921f9cd2aa895e8a9684c638bde69838
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912241"
---
# <a name="migrate-public-folder-data-to-microsoft-365"></a><span data-ttu-id="15895-102">ย้ายข้อมูลโฟลเดอร์สาธารณะไปยัง Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="15895-102">Migrate public folder data to Microsoft 365</span></span>

<span data-ttu-id="15895-103">ถ้าคุณไม่มีโฟลเดอร์สาธารณะจํานวนมากเพื่อนําเข้ามาใน Microsoft 365 วิธีที่ง่ายที่สุดที่จะนําพวกเขาคือการคัดลอกข้อมูลลงใน แฟ้ม PST แล้วนําเข้าลงใน Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="15895-103">If you don't have a lot of public folders to bring into Microsoft 365, the easiest way to bring them would be to copy the data into .PST files and then import them into Microsoft 365.</span></span> <span data-ttu-id="15895-104">สําหรับข้อมูลจํานวนเล็กน้อย แฟ้ม PST สามารถเพียงพอ</span><span class="sxs-lookup"><span data-stu-id="15895-104">For small amounts of data, a simple drag and drop of public folder into a .PST file can be sufficient.</span></span> <span data-ttu-id="15895-105">หากคุณมีข้อมูลมากกว่าที่ (ถึง 30GB), เราได้[จัดทําเอกสารกระบวนการ](https://technet.microsoft.com/library/dn874017%28v=exchg.150%29.aspx)ที่คุณสามารถใช้เพื่อส่งออกโฟลเดอร์ไปยังแฟ้ม PST.</span><span class="sxs-lookup"><span data-stu-id="15895-105">If you have more data than that (up to 30GB), we have [documented a process](https://technet.microsoft.com/library/dn874017%28v=exchg.150%29.aspx) that you can use to export folders to PST files.</span></span>
  
<span data-ttu-id="15895-106">สําหรับองค์กรขนาดใหญ่ที่กําลังย้ายโฟลเดอร์สาธารณะไปยัง Microsoft 365 เรามีคําแนะนําที่พร้อมใช้งาน:</span><span class="sxs-lookup"><span data-stu-id="15895-106">For larger organizations who are moving public folders into Microsoft 365, we have guides available:</span></span>
  
- <span data-ttu-id="15895-107">[โยกย้ายโฟลเดอร์สาธารณะแบบดั้งเดิม](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/batch-migration-of-legacy-public-folders)(Exchange 2010)</span><span class="sxs-lookup"><span data-stu-id="15895-107">[Migrate legacy public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/batch-migration-of-legacy-public-folders) (Exchange 2010)</span></span>

- [<span data-ttu-id="15895-108">โยกย้าย Exchange 2013, Exchange 2016 หรือ Exchange 2019 โฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="15895-108">Migrate Exchange 2013, Exchange 2016, or Exchange 2019 public folders</span></span>](https://docs.microsoft.com/Exchange/collaboration/public-folders/migrate-to-exchange-online)

<span data-ttu-id="15895-109">นอกจากนี้คุณยังมีตัวเลือกใน[การย้ายโฟลเดอร์สาธารณะไปยังกลุ่ม 365 Microsoft](https://docs.microsoft.com/Exchange/collaboration/public-folders/migrate-to-office-365-groups)</span><span class="sxs-lookup"><span data-stu-id="15895-109">You also have the option to [migrate public folders to Microsoft 365 Groups](https://docs.microsoft.com/Exchange/collaboration/public-folders/migrate-to-office-365-groups).</span></span>
  