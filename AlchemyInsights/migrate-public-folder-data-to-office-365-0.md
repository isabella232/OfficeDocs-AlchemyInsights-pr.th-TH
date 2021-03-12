---
title: โยกย้ายข้อมูลโฟลเดอร์สาธารณะไปยัง Microsoft 365
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "639"
- "3500007"
ms.assetid: 6e536c7d-ab36-413e-9702-63e51adb3452
ms.openlocfilehash: 6dac268b3371af3a28bf8ef598e3a74d954a595c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707325"
---
# <a name="migrate-public-folder-data-to-microsoft-365"></a><span data-ttu-id="0e4ad-102">โยกย้ายข้อมูลโฟลเดอร์สาธารณะไปยัง Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0e4ad-102">Migrate public folder data to Microsoft 365</span></span>

<span data-ttu-id="0e4ad-103">ถ้าคุณไม่มีโฟลเดอร์สาธารณะหลายโฟลเดอร์ให้ดาวน์โหลดลงใน Microsoft 365 วิธีที่ง่ายที่สุดในการเอาโฟลเดอร์เหล่านั้นมาคัดลอกข้อมูลลงใน ไฟล์ PST แล้วนําเข้าไฟล์ลงใน Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0e4ad-103">If you don't have a lot of public folders to bring into Microsoft 365, the easiest way to bring them would be to copy the data into .PST files and then import them into Microsoft 365.</span></span> <span data-ttu-id="0e4ad-104">ข้อมูลจํานวนน้อย ๆ คุณสามารถลากแล้วปล่อยโฟลเดอร์สาธารณะลงใน . ไฟล์ PST อาจเพียงพอ</span><span class="sxs-lookup"><span data-stu-id="0e4ad-104">For small amounts of data, a simple drag and drop of public folder into a .PST file can be sufficient.</span></span> <span data-ttu-id="0e4ad-105">ถ้าคุณมีข้อมูลมากกว่านั้น (สูงสุด 30 GB) เราได้บันทึกกระบวนการ [ที่คุณสามารถใช้เพื่อ](https://technet.microsoft.com/library/dn874017%28v=exchg.150%29.aspx) ส่งออกโฟลเดอร์ไปยังไฟล์ PST</span><span class="sxs-lookup"><span data-stu-id="0e4ad-105">If you have more data than that (up to 30GB), we have [documented a process](https://technet.microsoft.com/library/dn874017%28v=exchg.150%29.aspx) that you can use to export folders to PST files.</span></span>
  
<span data-ttu-id="0e4ad-106">For larger organizations who are moving public folders into Microsoft 365, we have guides available:</span><span class="sxs-lookup"><span data-stu-id="0e4ad-106">For larger organizations who are moving public folders into Microsoft 365, we have guides available:</span></span>
  
- <span data-ttu-id="0e4ad-107">[โยกย้ายโฟลเดอร์สาธารณะแบบดั้งเดิม](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/batch-migration-of-legacy-public-folders) (Exchange 2010)</span><span class="sxs-lookup"><span data-stu-id="0e4ad-107">[Migrate legacy public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/batch-migration-of-legacy-public-folders) (Exchange 2010)</span></span>

- [<span data-ttu-id="0e4ad-108">โยกย้ายโฟลเดอร์สาธารณะของ Exchange 2013, Exchange 2016 หรือ Exchange 2019</span><span class="sxs-lookup"><span data-stu-id="0e4ad-108">Migrate Exchange 2013, Exchange 2016, or Exchange 2019 public folders</span></span>](https://docs.microsoft.com/Exchange/collaboration/public-folders/migrate-to-exchange-online)

<span data-ttu-id="0e4ad-109">คุณยังมีตัวเลือกในการโยกย้าย[โฟลเดอร์สาธารณะไปยังกลุ่ม Microsoft 365](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/migrate-your-public-folders-to-microsoft-365-groups)</span><span class="sxs-lookup"><span data-stu-id="0e4ad-109">You also have the option to [migrate public folders to Microsoft 365 Groups](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/migrate-your-public-folders-to-microsoft-365-groups).</span></span>
  