---
title: ๑๔๙๐-การแก้ไขปัญหา-eDiscovery-ความล้มเหลว
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277834"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="3aa3f-102">การแก้ไขปัญหาข้อผิดพลาดในการค้นหาเนื้อหา</span><span class="sxs-lookup"><span data-stu-id="3aa3f-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="3aa3f-103">คุณพบปัญหาเกี่ยวกับการค้นหาเนื้อหาหรือความล้มเหลวเมื่อคุณส่งออกผลลัพธ์การค้นหาหรือไม่</span><span class="sxs-lookup"><span data-stu-id="3aa3f-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="3aa3f-104">ตัวอย่างเช่นคุณจะได้รับสิ่งต่อไปนี้เมื่อเรียกใช้การค้นหา</span><span class="sxs-lookup"><span data-stu-id="3aa3f-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="3aa3f-105">ข้อผิดพลาด CS008 หรือ CS012</span><span class="sxs-lookup"><span data-stu-id="3aa3f-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="3aa3f-106">ข้อผิดพลาดของเซิร์ฟเวอร์ไม่ว่าง/หมดเวลา</span><span class="sxs-lookup"><span data-stu-id="3aa3f-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="3aa3f-107">เกิดข้อผิดพลาดของแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="3aa3f-107">Application error occurred</span></span>

<span data-ttu-id="3aa3f-108">หรือเมื่อการค้นหาหรือส่งออกผลลัพธ์จากกล่องจดหมายจำนวนมาก (มากกว่ากล่องจดหมาย๑๐๐,๐๐๐) คุณจะได้รับข้อผิดพลาดในการส่งออกหรือไม่</span><span class="sxs-lookup"><span data-stu-id="3aa3f-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="3aa3f-109">สำหรับข้อผิดพลาดชนิดเหล่านี้ให้ลองค้นหาตำแหน่งที่ตั้งเนื้อหาที่ล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="3aa3f-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="3aa3f-110">ดู  [บทความนี้](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="3aa3f-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="3aa3f-111">ถ้าคุณกำลังส่งออกกล่องจดหมายมากกว่า100K คุณจะต้องใช้ Powershell ต่อไปนี้เพื่อดาวน์โหลดผลลัพธ์การส่งออก:[ส่งออกผลลัพธ์จากกล่องจดหมายมากกว่า 100k](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="3aa3f-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
