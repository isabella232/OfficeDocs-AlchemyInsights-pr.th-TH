---
title: แผนภูมิแสดงจำนวนระเบียนที่แตกต่างกันในเส้นตาราง
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793777"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="8bdcf-102">แผนภูมิแสดงจำนวนระเบียนที่แตกต่างกันในเส้นตาราง</span><span class="sxs-lookup"><span data-stu-id="8bdcf-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="8bdcf-103">**อาการ**</span><span class="sxs-lookup"><span data-stu-id="8bdcf-103">**Symptom**</span></span>

<span data-ttu-id="8bdcf-104">สำหรับแผนภูมิบนหน้าแดชบอร์ดเมื่อคุณคลิกที่แผนภูมิ "..." แล้วคลิก "ดูระเบียน" คุณสามารถนำทางไปยังหน้าเส้นตารางเพื่อดูระเบียนทั้งหมดได้ ในบางครั้งจำนวนระเบียนจะเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="8bdcf-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="8bdcf-105">**สาเหตุ**</span><span class="sxs-lookup"><span data-stu-id="8bdcf-105">**Cause**</span></span>

<span data-ttu-id="8bdcf-106">นี่คือเนื่องจากความแตกต่างของมุมมองระหว่างแผนภูมิบนหน้าแดชบอร์ดต้นฉบับและแผนภูมิบนหน้าแรกของเส้นตาราง</span><span class="sxs-lookup"><span data-stu-id="8bdcf-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="8bdcf-107">**วิธีแก้ไข**</span><span class="sxs-lookup"><span data-stu-id="8bdcf-107">**Solution**</span></span>

1. <span data-ttu-id="8bdcf-108">เลือกมุมมองจากหน้าต้นฉบับและมุมมองในตารางเพื่อดูว่าพวกเขาแตกต่างกันหรือไม่</span><span class="sxs-lookup"><span data-stu-id="8bdcf-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="8bdcf-109">เปลี่ยนมุมมองในตารางเพื่อให้ตรงกับมุมมองในหน้าต้นฉบับ</span><span class="sxs-lookup"><span data-stu-id="8bdcf-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="8bdcf-110">ถ้าไม่พบมุมมองที่ถูกต้องโดยปกติจะหมายความว่ามุมมองไม่ได้ถูกเปิดใช้งานในตัวออกแบบแอป</span><span class="sxs-lookup"><span data-stu-id="8bdcf-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="8bdcf-111">ไปที่ตัวออกแบบแอปของแอปที่เฉพาะเจาะจงเลือกเอนทิตีและมุมมองของแอปแล้วตรวจสอบมุมมองที่คุณต้องการเปิดใช้งานบันทึกประกาศและปิด</span><span class="sxs-lookup"><span data-stu-id="8bdcf-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="8bdcf-112">รีเฟรชหน้า</span><span class="sxs-lookup"><span data-stu-id="8bdcf-112">Refresh the page.</span></span>