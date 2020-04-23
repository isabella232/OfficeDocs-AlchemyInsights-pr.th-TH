---
title: รายการขนาดใหญ่ของ SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767304"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="b8570-102">ทํางานกับรายการและไลบรารีขนาดใหญ่ใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="b8570-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="b8570-103">รายการ SharePoint และไลบรารีสามารถมีได้ถึง 30 ล้านรายการ แต่เมื่อพวกเขามีมากกว่า 5,000 รายการ คุณอาจเห็นข้อผิดพลาดของเกณฑ์มุมมองรายการเมื่อคุณพยายามทํางานกับรายการเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="b8570-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="b8570-104">เกณฑ์นี้อยู่ในสถานที่เพื่อรักษาประสิทธิภาพของบริการ</span><span class="sxs-lookup"><span data-stu-id="b8570-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="b8570-105">มันไม่สามารถเปลี่ยนแปลงได้</span><span class="sxs-lookup"><span data-stu-id="b8570-105">It can't be changed.</span></span> <span data-ttu-id="b8570-106">วิธีหลีกเลี่ยงการกดปุ่มเกณฑ์นี้</span><span class="sxs-lookup"><span data-stu-id="b8570-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="b8570-107">**ใช้ทันสมัย**</span><span class="sxs-lookup"><span data-stu-id="b8570-107">**Use modern**</span></span>

<span data-ttu-id="b8570-108">มุมมองที่แสดงรายการจํานวนมากทํางานได้ดีที่สุดในประสบการณ์สมัยใหม่</span><span class="sxs-lookup"><span data-stu-id="b8570-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="b8570-109">[ใช้ประสบการณ์ที่ทันสมัย](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9)เพื่อหลีกเลี่ยงข้อผิดพลาดที่คุณอาจเห็นในประสบการณ์คลาสสิก</span><span class="sxs-lookup"><span data-stu-id="b8570-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="b8570-110">**เพิ่มดัชนี**</span><span class="sxs-lookup"><span data-stu-id="b8570-110">**Add indexes**</span></span>

<span data-ttu-id="b8570-111">เมื่อคุณกรองหรือเรียงลําดับตามคอลัมน์ที่ไม่มีดัชนี</span><span class="sxs-lookup"><span data-stu-id="b8570-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="b8570-112">[เพิ่มดัชนี](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0)ด้วยตนเองจาก**การตั้งค่ารายการ**ในเมนูการตั้งค่า แล้ว**คอลัมน์ที่จัดทําดัชนี**</span><span class="sxs-lookup"><span data-stu-id="b8570-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="b8570-113">**แก้ไขมุมมองรายการ**</span><span class="sxs-lookup"><span data-stu-id="b8570-113">**Edit the list view**</span></span>

<span data-ttu-id="b8570-114">ถ้ามีข้อผิดพลาดเกิดขึ้นเมื่อทํางานกับรายการขนาดใหญ่ ให้[แก้ไขมุมมองรายการของคุณ](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)</span><span class="sxs-lookup"><span data-stu-id="b8570-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="b8570-115">การเปลี่ยนแปลงสี่การเปลี่ยนแปลงต่อไปนี้จะเอาข้อผิดพลาดเกณฑ์มุมมองรายการออก</span><span class="sxs-lookup"><span data-stu-id="b8570-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="b8570-116">ทําการเปลี่ยนแปลงทั้งสี่เพื่อลบข้อผิดพลาดทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="b8570-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="b8570-117">ถ้าคุณยังคงได้รับข้อผิดพลาด ให้เลือก[จัดการรายการและไลบรารีขนาดใหญ่](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)</span><span class="sxs-lookup"><span data-stu-id="b8570-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="b8570-118">เลือก**ไม่มี**จากทั้งสอง**เรียงลําดับแรกตามคอลัมน์\*\*\*\*และ แล้วเรียงลําดับตามคอลัมน์**</span><span class="sxs-lookup"><span data-stu-id="b8570-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="b8570-119">เลือก**ไม่มี**จากทั้งสอง**กลุ่มแรกตามคอลัมน์\*\*\*\*และจัดกลุ่มตามคอลัมน์**</span><span class="sxs-lookup"><span data-stu-id="b8570-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="b8570-120">เลือก**ไม่มี**สําหรับคอลัมน์ทั้งหมดในส่วน**ผลรวม**</span><span class="sxs-lookup"><span data-stu-id="b8570-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="b8570-121">ยกเลิกการเลือกคอลัมน์ทั้งหมดแต่หนึ่งคอลัมน์สําหรับแสดงจากส่วน**คอลัมน์**</span><span class="sxs-lookup"><span data-stu-id="b8570-121">Deselect all but one column for display from the **Columns** section.</span></span>

