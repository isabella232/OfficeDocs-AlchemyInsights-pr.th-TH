---
title: รายการขนาดใหญ่ของ SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720152"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="91c4f-102">ทำงานกับรายการและไลบรารีขนาดใหญ่ใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="91c4f-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="91c4f-103">รายการและไลบรารี SharePoint สามารถมีได้ถึง๓๐,๐๐๐,๐๐๐รายการแต่เมื่อพวกเขามีรายการมากกว่า๕,๐๐๐คุณอาจเห็นข้อผิดพลาดเกณฑ์ของมุมมองรายการเมื่อคุณพยายามทำงานกับรายการเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="91c4f-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="91c4f-104">เกณฑ์นี้มีไว้เพื่อรักษาประสิทธิภาพการทำงานของบริการ</span><span class="sxs-lookup"><span data-stu-id="91c4f-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="91c4f-105">ไม่สามารถเปลี่ยนแปลงได้</span><span class="sxs-lookup"><span data-stu-id="91c4f-105">It can't be changed.</span></span> <span data-ttu-id="91c4f-106">เมื่อต้องการหลีกเลี่ยงการตีค่าเกณฑ์นี้:</span><span class="sxs-lookup"><span data-stu-id="91c4f-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="91c4f-107">**ใช้สมัยใหม่**</span><span class="sxs-lookup"><span data-stu-id="91c4f-107">**Use modern**</span></span>

<span data-ttu-id="91c4f-108">มุมมองที่แสดงรายการจำนวนมากทำงานได้ดีที่สุดในประสบการณ์การใช้งานที่ทันสมัย</span><span class="sxs-lookup"><span data-stu-id="91c4f-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="91c4f-109">[ใช้ประสบการณ์การใช้งานที่ทันสมัย](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) เพื่อหลีกเลี่ยงข้อผิดพลาดที่คุณอาจเห็นในประสบการณ์การใช้งานแบบคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="91c4f-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="91c4f-110">**เพิ่มดัชนี**</span><span class="sxs-lookup"><span data-stu-id="91c4f-110">**Add indexes**</span></span>

<span data-ttu-id="91c4f-111">เมื่อคุณกรองหรือเรียงลำดับตามคอลัมน์ที่ไม่มีดัชนีคุณอาจเห็นข้อความแสดงข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="91c4f-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="91c4f-112">[เพิ่มดัชนี](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0)ด้วยตนเองจาก**การตั้งค่ารายการ**ในเมนูการตั้งค่าจากนั้นเลือกคอลัมน์ที่มีการทำ**ดัชนี**</span><span class="sxs-lookup"><span data-stu-id="91c4f-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="91c4f-113">**แก้ไขมุมมองรายการ**</span><span class="sxs-lookup"><span data-stu-id="91c4f-113">**Edit the list view**</span></span>

<span data-ttu-id="91c4f-114">ถ้ามีข้อผิดพลาดเกิดขึ้นเมื่อทำงานกับรายการขนาดใหญ่ให้[แก้ไขมุมมองรายการของคุณ](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)</span><span class="sxs-lookup"><span data-stu-id="91c4f-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="91c4f-115">การเปลี่ยนแปลงสี่รายการต่อไปนี้จะเอาข้อผิดพลาดขีดจำกัดของมุมมองรายการออก</span><span class="sxs-lookup"><span data-stu-id="91c4f-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="91c4f-116">ทำการเปลี่ยนแปลงทั้งสี่เพื่อเอาข้อผิดพลาดทั้งหมดออก</span><span class="sxs-lookup"><span data-stu-id="91c4f-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="91c4f-117">ถ้าคุณยังคงได้รับข้อผิดพลาดให้ตรวจสอบ[จัดการรายการและไลบรารีขนาดใหญ่](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)</span><span class="sxs-lookup"><span data-stu-id="91c4f-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="91c4f-118">เลือก**ไม่มี**จากทั้งสอง**เรียงลำดับตามคอลัมน์**แล้ว**เรียงลำดับตามคอลัมน์**</span><span class="sxs-lookup"><span data-stu-id="91c4f-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="91c4f-119">เลือก**ไม่มี**จากทั้ง**กลุ่มแรกตามคอลัมน์**แล้ว**จัดกลุ่มตามคอลัมน์**</span><span class="sxs-lookup"><span data-stu-id="91c4f-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="91c4f-120">เลือก**ไม่มี**สำหรับคอลัมน์ทั้งหมดในส่วน**ผลรวม**</span><span class="sxs-lookup"><span data-stu-id="91c4f-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="91c4f-121">ยกเลิกการเลือกคอลัมน์ทั้งหมดแต่หนึ่งคอลัมน์เพื่อแสดงจากส่วน**คอลัมน์**</span><span class="sxs-lookup"><span data-stu-id="91c4f-121">Deselect all but one column for display from the **Columns** section.</span></span>

