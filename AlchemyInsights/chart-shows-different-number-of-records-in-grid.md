---
title: แผนภูมิแสดงจํานวนระเบียนที่แตกต่างกันในตาราง
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439960"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="b8df3-102">แผนภูมิแสดงจํานวนระเบียนที่แตกต่างกันในตาราง</span><span class="sxs-lookup"><span data-stu-id="b8df3-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="b8df3-103">**อาการ**</span><span class="sxs-lookup"><span data-stu-id="b8df3-103">**Symptom**</span></span>

<span data-ttu-id="b8df3-104">สําหรับแผนภูมิในหน้าแดชบอร์ดเมื่อคุณคลิกที่แผนภูมิ "..." และคลิก "ดูระเบียน" คุณนําทางไปยังหน้าตารางเพื่อดูระเบียนทั้งหมด บางครั้งจํานวนระเบียนจะเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="b8df3-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="b8df3-105">**สาเหตุ**</span><span class="sxs-lookup"><span data-stu-id="b8df3-105">**Cause**</span></span>

<span data-ttu-id="b8df3-106">นี่คือสาเหตุที่ความแตกต่างของมุมมองระหว่างแผนภูมิบนหน้าแดชบอร์ดเดิมและแผนภูมิบนโฮมเพจของกริด</span><span class="sxs-lookup"><span data-stu-id="b8df3-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="b8df3-107">**โซลูชัน**</span><span class="sxs-lookup"><span data-stu-id="b8df3-107">**Solution**</span></span>

1. <span data-ttu-id="b8df3-108">ตรวจสอบมุมมองจากหน้าต้นฉบับและมุมมองในตารางเพื่อดูว่ามีความแตกต่างกันหรือไม่</span><span class="sxs-lookup"><span data-stu-id="b8df3-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="b8df3-109">เปลี่ยนมุมมองในกริดให้ตรงกับมุมมองในหน้าต้นฉบับ</span><span class="sxs-lookup"><span data-stu-id="b8df3-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="b8df3-110">หากไม่พบมุมมองที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="b8df3-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="b8df3-111">ไปที่ตัวออกแบบแอปของแอปเฉพาะให้เลือกเอนทิตีและมุมมองของเอนทิตีตรวจสอบมุมมองที่คุณต้องการเปิดใช้งานบันทึกเผยแพร่และปิด</span><span class="sxs-lookup"><span data-stu-id="b8df3-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="b8df3-112">รีเฟรชหน้า</span><span class="sxs-lookup"><span data-stu-id="b8df3-112">Refresh the page.</span></span>