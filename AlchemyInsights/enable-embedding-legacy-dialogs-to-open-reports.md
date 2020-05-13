---
title: เปิดใช้งานการฝังกล่องโต้ตอบแบบดั้งเดิมเพื่อเปิดรายงาน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: ca0894849e95fd69acd2065c3f065547231a07f9
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204678"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="f7265-102">เปิดใช้งานการฝังกล่องโต้ตอบแบบดั้งเดิมเพื่อเปิดรายงาน</span><span class="sxs-lookup"><span data-stu-id="f7265-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="f7265-103">**อาการ**</span><span class="sxs-lookup"><span data-stu-id="f7265-103">**Symptom**</span></span>

<span data-ttu-id="f7265-104">ผู้ใช้ไม่สามารถเปิดรายงานได้</span><span class="sxs-lookup"><span data-stu-id="f7265-104">Users are unable to open reports.</span></span> <span data-ttu-id="f7265-105">"มีบางอย่างผิดปกติ</span><span class="sxs-lookup"><span data-stu-id="f7265-105">"Something has gone wrong.</span></span> <span data-ttu-id="f7265-106">ตรวจสอบรายละเอียดทางเทคนิคสําหรับรายละเอียดเพิ่มเติม"</span><span class="sxs-lookup"><span data-stu-id="f7265-106">Check technical details for more details."</span></span>

<span data-ttu-id="f7265-107">**สาเหตุ**</span><span class="sxs-lookup"><span data-stu-id="f7265-107">**Cause**</span></span>

<span data-ttu-id="f7265-108">รายงานจะล้มเหลวในการโหลดใน UCI มีข้อผิดพลาด "ตัวบอกลักษณะแบบฟอร์มเป็น null หรือไม่ได้กําหนด"</span><span class="sxs-lookup"><span data-stu-id="f7265-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="f7265-109">รายงานใน UCI ยังคงต้องการกล่องโต้ตอบแบบดั้งเดิม ดังนั้นระบบของลูกค้าจึงจําเป็นต้องเปิดใช้งาน*allowlegacydialogsembedding*</span><span class="sxs-lookup"><span data-stu-id="f7265-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="f7265-110">**โซลูชัน**</span><span class="sxs-lookup"><span data-stu-id="f7265-110">**Solution**</span></span>

1. <span data-ttu-id="f7265-111">ไปที่**การตั้งค่า>การจัดการ> > แท็บ ทั่วไป**</span><span class="sxs-lookup"><span data-stu-id="f7265-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="f7265-112">ตั้งค่า "เปิดใช้งานการฝังกล่องโต้ตอบดั้งเดิมบางอย่างในไคลเอ็นต์เบราว์เซอร์ส่วนติดต่อแบบรวม" เป็น**ใช่**</span><span class="sxs-lookup"><span data-stu-id="f7265-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
