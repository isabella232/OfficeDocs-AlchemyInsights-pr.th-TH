---
title: เปิดใช้งานกล่องโต้ตอบการฝังแบบดั้งเดิมเพื่อเปิดรายงาน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806454"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="7042d-102">เปิดใช้งานกล่องโต้ตอบการฝังแบบดั้งเดิมเพื่อเปิดรายงาน</span><span class="sxs-lookup"><span data-stu-id="7042d-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="7042d-103">**อาการ**</span><span class="sxs-lookup"><span data-stu-id="7042d-103">**Symptom**</span></span>

<span data-ttu-id="7042d-104">ผู้ใช้ไม่สามารถเปิดรายงานได้</span><span class="sxs-lookup"><span data-stu-id="7042d-104">Users are unable to open reports.</span></span> <span data-ttu-id="7042d-105">"มีบางอย่างผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="7042d-105">"Something has gone wrong.</span></span> <span data-ttu-id="7042d-106">ตรวจสอบรายละเอียดทางเทคนิคสำหรับรายละเอียดเพิ่มเติม "</span><span class="sxs-lookup"><span data-stu-id="7042d-106">Check technical details for more details."</span></span>

<span data-ttu-id="7042d-107">**สาเหตุ**</span><span class="sxs-lookup"><span data-stu-id="7042d-107">**Cause**</span></span>

<span data-ttu-id="7042d-108">รายงานจะล้มเหลวในการโหลดใน UCI ที่มีข้อผิดพลาด "ตัวอธิบายฟอร์มเป็น null หรือไม่ได้กำหนดไว้"</span><span class="sxs-lookup"><span data-stu-id="7042d-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="7042d-109">รายงานใน UCI ยังจำเป็นต้องมีกล่องโต้ตอบแบบดั้งเดิมดังนั้นระบบของลูกค้าจึงจำเป็นต้องมีการเปิดใช้งาน*allowlegacydialogsembedding*</span><span class="sxs-lookup"><span data-stu-id="7042d-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="7042d-110">**วิธีแก้ไข**</span><span class="sxs-lookup"><span data-stu-id="7042d-110">**Solution**</span></span>

1. <span data-ttu-id="7042d-111">ไปที่การ**ตั้งค่า >การตั้งค่าระบบ > การดูแลระบบ > แท็บทั่วไป**</span><span class="sxs-lookup"><span data-stu-id="7042d-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="7042d-112">ตั้งค่า "เปิดใช้งานการฝังของกล่องโต้ตอบแบบดั้งเดิมบางรายการในไคลเอ็นต์เบราว์เซอร์ส่วนติดต่อ" เป็น**ใช่**</span><span class="sxs-lookup"><span data-stu-id="7042d-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
