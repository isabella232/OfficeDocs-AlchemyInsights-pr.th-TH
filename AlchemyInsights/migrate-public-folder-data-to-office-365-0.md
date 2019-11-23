---
title: ย้ายข้อมูลโฟลเดอร์สาธารณะไปยัง Office ๓๖๕
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
ms.openlocfilehash: 85bef3ac5f590a57ead16cb73c7961fcb0ee8eae
ms.sourcegitcommit: 198defbbed20dd9db3f7c044c6e77a8feb05dacd
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/22/2019
ms.locfileid: "39202613"
---
# <a name="migrate-public-folder-data-to-office-365"></a><span data-ttu-id="8a722-102">ย้ายข้อมูลโฟลเดอร์สาธารณะไปยัง Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="8a722-102">Migrate public folder data to Office 365</span></span>

<span data-ttu-id="8a722-103">ถ้าคุณไม่มีโฟลเดอร์สาธารณะจำนวนมากที่จะนำเข้ามาใน Office ๓๖๕วิธีที่ง่ายที่สุดที่จะนำพวกเขาจะทำสำเนาข้อมูลลงไป แฟ้ม PST และนำเข้าไปยัง Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="8a722-103">If you don't have a lot of public folders to bring into Office 365, the easiest way to bring them would be to copy the data into .PST files and then import them into Office 365.</span></span> <span data-ttu-id="8a722-104">สำหรับข้อมูลจำนวนน้อยให้ลากและวางโฟลเดอร์สาธารณะแบบง่ายๆลงใน ไฟล์ PST สามารถเพียงพอ.</span><span class="sxs-lookup"><span data-stu-id="8a722-104">For small amounts of data, a simple drag and drop of public folder into a .PST file can be sufficient.</span></span> <span data-ttu-id="8a722-105">หากคุณมีข้อมูลมากกว่านั้น (ไม่เกิน 30GB) เราได้จัดทำ[เอกสารกระบวนการ](https://technet.microsoft.com/library/dn874017%28v=exchg.150%29.aspx)ที่คุณสามารถใช้เพื่อส่งออกโฟลเดอร์ไปยังแฟ้ม PST</span><span class="sxs-lookup"><span data-stu-id="8a722-105">If you have more data than that (up to 30GB), we have [documented a process](https://technet.microsoft.com/library/dn874017%28v=exchg.150%29.aspx) that you can use to export folders to PST files.</span></span>
  
<span data-ttu-id="8a722-106">สำหรับองค์กรขนาดใหญ่ที่กำลังย้ายโฟลเดอร์สาธารณะไปยัง Office ๓๖๕เรามีคำแนะนำที่พร้อมใช้งาน:</span><span class="sxs-lookup"><span data-stu-id="8a722-106">For larger organizations who are moving public folders into Office 365, we have guides available:</span></span>
  
- <span data-ttu-id="8a722-107">[โยกย้ายโฟลเดอร์สาธารณะดั้งเดิม](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/batch-migration-of-legacy-public-folders)(Exchange ๒๐๑๐)</span><span class="sxs-lookup"><span data-stu-id="8a722-107">[Migrate legacy public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/batch-migration-of-legacy-public-folders) (Exchange 2010)</span></span>

- [<span data-ttu-id="8a722-108">ย้ายข้อมูล Exchange ๒๐๑๓อัตราแลกเปลี่ยน๒๐๑๖หรือ Exchange ๒๐๑๙โฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="8a722-108">Migrate Exchange 2013, Exchange 2016, or Exchange 2019 public folders</span></span>](https://docs.microsoft.com/Exchange/collaboration/public-folders/migrate-to-exchange-online)

<span data-ttu-id="8a722-109">นอกจากนี้คุณยังมีตัวเลือกในการ[ย้ายโฟลเดอร์สาธารณะไปยัง Office ๓๖๕กลุ่ม](https://docs.microsoft.com/Exchange/collaboration/public-folders/migrate-to-office-365-groups)</span><span class="sxs-lookup"><span data-stu-id="8a722-109">You also have the option to [migrate public folders to Office 365 Groups](https://docs.microsoft.com/Exchange/collaboration/public-folders/migrate-to-office-365-groups).</span></span>
  