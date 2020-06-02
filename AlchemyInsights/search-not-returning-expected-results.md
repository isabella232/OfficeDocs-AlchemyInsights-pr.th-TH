---
title: 1491-ค้นหา-ไม่ส่งกลับผลลัพธ์ที่คาดหวัง
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510591"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="ef8d7-102">การค้นหาเนื้อหาไม่ส่งกลับผลลัพธ์ที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="ef8d7-102">Content Search not returning expected results</span></span>

<span data-ttu-id="ef8d7-103">เมื่อเรียกใช้การค้นหาเนื้อหาจากความปลอดภัยของ Microsoft 365 &ศูนย์การปฏิบัติตามกฎระเบียบ คุณอาจได้รับผลลัพธ์การค้นหาที่ไม่คาดคิด</span><span class="sxs-lookup"><span data-stu-id="ef8d7-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="ef8d7-104">พิจารณาสิ่งต่อไปนี้ที่อาจส่งผลต่อผลการค้นหาของคุณ</span><span class="sxs-lookup"><span data-stu-id="ef8d7-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="ef8d7-105">**ตําแหน่งที่ตั้งเนื้อหาและเงื่อนไขการค้นหา**: ตรวจสอบให้แน่ใจว่าคุณได้เลือกตําแหน่งที่ตั้งเนื้อหาและเงื่อนไขการค้นหาที่เหมาะสมแล้ว</span><span class="sxs-lookup"><span data-stu-id="ef8d7-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="ef8d7-106">หากคุณเรียกใช้การค้นหาขนาดใหญ่ (ที่มีหลายตําแหน่ง) ให้ลองแยกการค้นหาออกเป็นการค้นหาหลายรายการ</span><span class="sxs-lookup"><span data-stu-id="ef8d7-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="ef8d7-107">**รายการที่ทําดัชนีบางส่วน**:[รายการบางส่วนที่มีการทําดัชนี](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search)จากกล่องจดหมายจะรวมอยู่ในผลลัพธ์การค้นหาโดยประมาณ</span><span class="sxs-lookup"><span data-stu-id="ef8d7-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="ef8d7-108">อย่างไรก็ตาม รายการที่ทําดัชนีบางส่วนจากไซต์ใน SharePoint และ OneDrive จะไม่รวมอยู่ในค่าประมาณการค้นหา</span><span class="sxs-lookup"><span data-stu-id="ef8d7-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="ef8d7-109">**ความล้มเหลวในการค้นหา**: เมื่อค้นหากล่องจดหมายจํานวนมาก (กล่องจดหมายมากกว่า 100,000) คุณอาจได้รับข้อผิดพลาดในการค้นหา ด้วยรหัสข้อผิดพลาดเช่น CS008-009 และ CS012-002)</span><span class="sxs-lookup"><span data-stu-id="ef8d7-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="ef8d7-110">ในกรณีนี้ ให้ลองค้นหาสําหรับตําแหน่งที่ตั้งเนื้อหาที่ล้มเหลวเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="ef8d7-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="ef8d7-111">ดู[บทความนี้](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="ef8d7-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
