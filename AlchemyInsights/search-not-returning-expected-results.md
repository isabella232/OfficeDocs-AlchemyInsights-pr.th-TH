---
title: 1491-ค้นหาไม่ส่งคืนผลลัพธ์ที่คาดไว้
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
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709246"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="297a1-102">การค้นหาเนื้อหาไม่ส่งกลับผลลัพธ์ที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="297a1-102">Content Search not returning expected results</span></span>

<span data-ttu-id="297a1-103">เมื่อเรียกใช้การค้นหาเนื้อหาจาก Microsoft 365 &ศูนย์การปฏิบัติตามกฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="297a1-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="297a1-104">พิจารณาสิ่งต่อไปนี้ที่อาจส่งผลต่อผลการค้นหาของคุณ</span><span class="sxs-lookup"><span data-stu-id="297a1-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="297a1-105">**ตําแหน่งที่ตั้งเนื้อหาและเงื่อนไขการค้นหา**: ตรวจสอบให้แน่ใจว่าคุณได้เลือกตําแหน่งเนื้อหาที่เหมาะสมและเงื่อนไขการค้นหา</span><span class="sxs-lookup"><span data-stu-id="297a1-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="297a1-106">หากคุณค้นหาข้อมูลจํานวนมาก (ที่มีหลายตําแหน่ง) ให้พิจารณาแยกการค้นหาออกเป็นหลายการค้นหา</span><span class="sxs-lookup"><span data-stu-id="297a1-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="297a1-107">**รายการที่มีการทําดัชนีบางส่วน**:[รายการทําดัชนีบางส่วน](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)จากกล่องจดหมายจะรวมอยู่ในผลลัพธ์การค้นหาโดยประมาณ</span><span class="sxs-lookup"><span data-stu-id="297a1-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="297a1-108">อย่างไรก็ตาม รายการทําดัชนีบางส่วนจากไซต์ใน SharePoint และ OneDrive จะไม่รวมอยู่ในการประเมินการค้นหา</span><span class="sxs-lookup"><span data-stu-id="297a1-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="297a1-109">**ความล้มเหลวในการค้นหา**: เมื่อค้นหากล่องจดหมายจํานวนมาก (กล่องจดหมายมากกว่า 100,000 กล่อง) คุณอาจได้รับข้อผิดพลาดในการค้นหาที่มีรหัสข้อผิดพลาดเช่น CS008-009 และ CS012-002)</span><span class="sxs-lookup"><span data-stu-id="297a1-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="297a1-110">ในกรณีนี้ ให้ลองค้นหาสําหรับตําแหน่งที่ตั้งเนื้อหาที่ล้มเหลวเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="297a1-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="297a1-111">ดู[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="297a1-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
