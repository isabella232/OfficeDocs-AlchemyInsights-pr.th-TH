---
title: เปิดใช้งานการฝังกล่องโต้ตอบแบบดั้งเดิมเพื่อเปิดรายงาน
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814283"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="d1ce6-102">เปิดใช้งานการฝังกล่องโต้ตอบแบบดั้งเดิมเพื่อเปิดรายงาน</span><span class="sxs-lookup"><span data-stu-id="d1ce6-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="d1ce6-103">**อาการ**</span><span class="sxs-lookup"><span data-stu-id="d1ce6-103">**Symptom**</span></span>

<span data-ttu-id="d1ce6-104">ผู้ใช้ไม่สามารถเปิดรายงานได้</span><span class="sxs-lookup"><span data-stu-id="d1ce6-104">Users are unable to open reports.</span></span> <span data-ttu-id="d1ce6-105">"มีบางอย่างผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="d1ce6-105">"Something has gone wrong.</span></span> <span data-ttu-id="d1ce6-106">ตรวจสอบรายละเอียดด้านเทคนิคเพื่อดูรายละเอียดเพิ่มเติม"</span><span class="sxs-lookup"><span data-stu-id="d1ce6-106">Check technical details for more details."</span></span>

<span data-ttu-id="d1ce6-107">**สาเหตุ**</span><span class="sxs-lookup"><span data-stu-id="d1ce6-107">**Cause**</span></span>

<span data-ttu-id="d1ce6-108">รายงานไม่สามารถโหลดใน UCI ที่มีข้อผิดพลาด "Form descriptor เป็น null หรือไม่ได้กําหนด"</span><span class="sxs-lookup"><span data-stu-id="d1ce6-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="d1ce6-109">รายงานใน UCI ยังต้องใช้กล่องโต้ตอบแบบดั้งเดิม ดังนั้นระบบของลูกค้าต้อง *เปิดใช้งาน allowlegacydialogsembeม*</span><span class="sxs-lookup"><span data-stu-id="d1ce6-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="d1ce6-110">**วิธีแก้ไข**</span><span class="sxs-lookup"><span data-stu-id="d1ce6-110">**Solution**</span></span>

1. <span data-ttu-id="d1ce6-111">ไปที่ การตั้งค่า **>การดูแล> การตั้งค่า> บนแท็บ** ทั่วไป</span><span class="sxs-lookup"><span data-stu-id="d1ce6-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="d1ce6-112">ตั้งค่า "เปิดใช้งานการฝังของกล่องโต้ตอบดั้งเดิมบางรายการในไคลเอ็นต์เบราว์เซอร์ส่วนติดต่อแบบรวม" **เป็น** ใช่</span><span class="sxs-lookup"><span data-stu-id="d1ce6-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
