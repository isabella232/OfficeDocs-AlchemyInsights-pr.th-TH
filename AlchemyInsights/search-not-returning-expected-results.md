---
title: ๑๔๙๑-การค้นหา-ไม่ใช่-การส่งกลับ-ผลลัพธ์ที่คาดไว้
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
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740493"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="279f4-102">การค้นหาเนื้อหาไม่ส่งกลับผลลัพธ์ที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="279f4-102">Content Search not returning expected results</span></span>

<span data-ttu-id="279f4-103">เมื่อเรียกใช้การค้นหาเนื้อหาจากศูนย์การปฏิบัติตามนโยบายของ Microsoft ๓๖๕ security & คุณอาจได้รับผลลัพธ์การค้นหาที่ไม่คาดคิด</span><span class="sxs-lookup"><span data-stu-id="279f4-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="279f4-104">พิจารณาสิ่งต่อไปนี้ที่สามารถส่งผลต่อผลลัพธ์การค้นหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="279f4-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="279f4-105">**ตำแหน่งที่ตั้งเนื้อหาและเงื่อนไขการค้นหา**: ตรวจสอบให้แน่ใจว่าคุณได้เลือกตำแหน่งที่ตั้งเนื้อหาที่เหมาะสมและเงื่อนไขการค้นหา</span><span class="sxs-lookup"><span data-stu-id="279f4-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="279f4-106">ถ้าคุณเรียกใช้การค้นหาขนาดใหญ่ (ที่มีตำแหน่งที่ตั้งจำนวนมาก) ให้พิจารณาแยกออกเป็นการค้นหาหลายรายการ</span><span class="sxs-lookup"><span data-stu-id="279f4-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="279f4-107">รายการที่มีการทำ**ดัชนีบางส่วน**: รายการที่มีการทำ[ดัชนีบางส่วน](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search)จากกล่องจดหมายจะรวมอยู่ในผลลัพธ์การค้นหาโดยประมาณ</span><span class="sxs-lookup"><span data-stu-id="279f4-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="279f4-108">อย่างไรก็ตามรายการที่มีการทำดัชนีบางส่วนจากไซต์ใน SharePoint และ OneDrive จะไม่รวมอยู่ในการประเมินการค้นหา</span><span class="sxs-lookup"><span data-stu-id="279f4-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="279f4-109">ความ**ล้มเหลวในการค้นหา**: เมื่อค้นหากล่องจดหมายจำนวนมาก (มากกว่ากล่องจดหมาย๑๐๐,๐๐๐) คุณอาจได้รับข้อผิดพลาดในการค้นหาด้วยรหัสข้อผิดพลาดเช่น CS008 และ CS012-002)</span><span class="sxs-lookup"><span data-stu-id="279f4-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="279f4-110">ในกรณีนี้ให้ลองใช้การค้นหาสำหรับตำแหน่งที่ตั้งเนื้อหาที่ล้มเหลวเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="279f4-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="279f4-111">ดู  [บทความนี้](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="279f4-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
