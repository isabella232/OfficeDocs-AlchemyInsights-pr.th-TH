---
title: ปรับใช้หลักปฏิบัติที่ดีที่สุดกับคิวรีการค้นหาขั้นสูงในการหาข้อมูล
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696081"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="7624d-102">ปรับใช้หลักปฏิบัติที่ดีที่สุดกับคิวรีการค้นหาขั้นสูงในการหาข้อมูล</span><span class="sxs-lookup"><span data-stu-id="7624d-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="7624d-103">เมื่อต้องการให้ผลลัพธ์เร็วขึ้นและหลีกเลี่ยงการหมดเวลาขณะใช้งานคิวรีที่ซับซ้อน ให้ปรับใช้หลักปฏิบัติที่ดีที่สุดเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="7624d-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="7624d-104">เมื่อลองคิวรีใหม่ ให้ใช้ขีดจํากัดเสมอเพื่อหลีกเลี่ยงชุดผลลัพธ์ที่มีขนาดใหญ่มาก</span><span class="sxs-lookup"><span data-stu-id="7624d-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="7624d-105">นอกจากนี้ `count` ยังใช้สร้างแบบประเมินเริ่มต้นของขนาดของชุดผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="7624d-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="7624d-106">ใช้ตัวกรองเวลาก่อน</span><span class="sxs-lookup"><span data-stu-id="7624d-106">Use time filters first.</span></span> <span data-ttu-id="7624d-107">ให้จํากัดคิวรีของคุณสูงสุดเจ็ดวัน</span><span class="sxs-lookup"><span data-stu-id="7624d-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="7624d-108">ในจุดเริ่มต้นของคิวรี หลังตัวกรองเวลา ให้เพิ่มตัวกรองที่คาดว่าจะเอาข้อมูลส่วนใหญ่ออก</span><span class="sxs-lookup"><span data-stu-id="7624d-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="7624d-109">เมื่อค้นหาโทเค็นแบบเต็ม ให้ใช้ตัว `has` ตัวการ `contains` แทน</span><span class="sxs-lookup"><span data-stu-id="7624d-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="7624d-110">เรียกใช้การค้นหาในคอลัมน์ใดคอลัมน์หนึ่งแทนที่จะเรียกใช้ในคอลัมน์ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="7624d-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="7624d-111">เมื่อรวมตาราง ก่อนอื่นให้ระบุตารางที่มีแถวน้อยกว่า</span><span class="sxs-lookup"><span data-stu-id="7624d-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="7624d-112">`project` เฉพาะคอลัมน์ที่จําเป็นจากตารางที่คุณได้รวมเข้าด้วยกัน</span><span class="sxs-lookup"><span data-stu-id="7624d-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="7624d-113">To learn more, see [Advanced query practices best](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="7624d-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
