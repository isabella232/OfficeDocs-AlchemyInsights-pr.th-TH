---
title: รายการขนาดใหญ่ของ SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488536"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="3134c-102">ทำงานกับรายการและไลบรารีขนาดใหญ่ใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="3134c-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="3134c-103">รายการและไลบรารีของ SharePoint สามารถมีได้ถึง๓๐,๐๐๐,๐๐๐รายการแต่เมื่อพวกเขามีมากกว่า๕,๐๐๐รายการคุณอาจเห็นข้อผิดพลาด Threshold มุมมองรายการเมื่อคุณพยายามที่จะทำงานกับพวกเขา</span><span class="sxs-lookup"><span data-stu-id="3134c-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="3134c-104">ขีดจำกัดนี้อยู่ในสถานที่เพื่อรักษาประสิทธิภาพการทำงานของการบริการ</span><span class="sxs-lookup"><span data-stu-id="3134c-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="3134c-105">ไม่สามารถเปลี่ยนแปลงได้</span><span class="sxs-lookup"><span data-stu-id="3134c-105">It can't be changed.</span></span> <span data-ttu-id="3134c-106">เพื่อหลีกเลี่ยงการกดปุ่มขีดจำกัดนี้:</span><span class="sxs-lookup"><span data-stu-id="3134c-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="3134c-107">**ใช้งานที่ทันสมัย**</span><span class="sxs-lookup"><span data-stu-id="3134c-107">**Use modern**</span></span>

<span data-ttu-id="3134c-108">มุมมองที่แสดงหลายรายการทำงานได้ดีที่สุดในประสบการณ์ที่ทันสมัย</span><span class="sxs-lookup"><span data-stu-id="3134c-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="3134c-109">[ใช้ประสบการณ์ที่ทันสมัย](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9)เพื่อหลีกเลี่ยงข้อผิดพลาดที่คุณอาจเห็นในประสบการณ์คลาสสิก</span><span class="sxs-lookup"><span data-stu-id="3134c-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="3134c-110">**เพิ่มดัชนี**</span><span class="sxs-lookup"><span data-stu-id="3134c-110">**Add indexes**</span></span>

<span data-ttu-id="3134c-111">เมื่อคุณกรองหรือเรียงลำดับตามคอลัมน์ที่ไม่มีดัชนีคุณอาจเห็นข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="3134c-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="3134c-112">[เพิ่มดัชนี](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0)ด้วยตนเองจาก**การตั้งค่ารายการ**ในเมนูการตั้งค่าจากนั้นทำ**ดัชนีคอลัมน์**</span><span class="sxs-lookup"><span data-stu-id="3134c-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="3134c-113">**แก้ไขมุมมองรายการ**</span><span class="sxs-lookup"><span data-stu-id="3134c-113">**Edit the list view**</span></span>

<span data-ttu-id="3134c-114">หากมีข้อผิดพลาดเกิดขึ้นขณะทำงานกับรายการขนาดใหญ่ให้[แก้ไขมุมมองรายการของคุณ](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)</span><span class="sxs-lookup"><span data-stu-id="3134c-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="3134c-115">การเปลี่ยนแปลงสี่รายการต่อไปนี้จะเอาข้อผิดพลาด threshold ของมุมมองรายชื่อออก</span><span class="sxs-lookup"><span data-stu-id="3134c-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="3134c-116">ทำการเปลี่ยนแปลงทั้งหมดสี่รายการเพื่อลบข้อผิดพลาดทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="3134c-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="3134c-117">หากคุณยังคงได้รับข้อผิดพลาดให้ตรวจสอบ[จัดการรายการและไลบรารีขนาดใหญ่](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)</span><span class="sxs-lookup"><span data-stu-id="3134c-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="3134c-118">เลือก**ไม่มี**จากทั้ง**เรียงลำดับแรกตามคอลัมน์**และ**เรียงลำดับตามคอลัมน์**</span><span class="sxs-lookup"><span data-stu-id="3134c-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="3134c-119">เลือก**ไม่มี**จากทั้ง**กลุ่มแรกตามคอลัมน์**แล้ว**จัดกลุ่มตามคอลัมน์**</span><span class="sxs-lookup"><span data-stu-id="3134c-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="3134c-120">เลือก**ไม่มี**สำหรับคอลัมน์ทั้งหมดในส่วน**ผลรวม**</span><span class="sxs-lookup"><span data-stu-id="3134c-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="3134c-121">ยกเลิกการเลือกทั้งหมดแต่คอลัมน์เดียวสำหรับการแสดงผลจากส่วน**คอลัมน์**</span><span class="sxs-lookup"><span data-stu-id="3134c-121">Deselect all but one column for display from the **Columns** section.</span></span>

