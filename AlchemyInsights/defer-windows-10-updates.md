---
title: การอัปเดต Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1128"
- "6700007"
ms.openlocfilehash: 233354386eb319860f25b3929b6be528438cc865
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680442"
---
# <a name="defer-windows-10-updates"></a><span data-ttu-id="d2ffb-102">การอัปเดต Windows 10</span><span class="sxs-lookup"><span data-stu-id="d2ffb-102">Defer Windows 10 updates</span></span>

<span data-ttu-id="d2ffb-103">เมื่อต้องการเลื่อนการอัปเดต Windows 10 ที่ผลักดันให้ผู้ใช้ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="d2ffb-103">To defer the Windows 10 updates pushed to users, follow these steps:</span></span>

1. <span data-ttu-id="d2ffb-104">ลงชื่อเข้าใช้พอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="d2ffb-104">Sign in to the Azure portal.</span></span>
2. <span data-ttu-id="d2ffb-105">เลือกการ**อัปเดตซอฟต์แวร์**   >   **Windows 10 การอัปเดตวงแหวน**</span><span class="sxs-lookup"><span data-stu-id="d2ffb-105">Select  **Software Updates**  >  **Windows 10 Update Rings**.</span></span>
3. <span data-ttu-id="d2ffb-106">ถ้าคุณไม่มีวงแหวนอัปเดตให้เลือกตัวเลือกเพื่อสร้างการตั้งค่าใหม่</span><span class="sxs-lookup"><span data-stu-id="d2ffb-106">If you don't have an update ring, select the option to create a new one.</span></span>
4. <span data-ttu-id="d2ffb-107">ใส่ชื่อและคำอธิบายเพิ่มเติมแล้วเลือก  **การตั้งค่าการตั้ง**ค่า</span><span class="sxs-lookup"><span data-stu-id="d2ffb-107">Enter a name and optional description, and then select  **Settings Configure**.</span></span>
5. <span data-ttu-id="d2ffb-108">กำหนดกรอบเวลาสำหรับการอัปเดเลื่อนที่แตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="d2ffb-108">Customize the timeframe for deferring different updates.</span></span> <span data-ttu-id="d2ffb-109">เวลารอการตัดบัญชีสูงสุดจะขึ้นอยู่กับชนิดของการอัปเดต:</span><span class="sxs-lookup"><span data-stu-id="d2ffb-109">Maximum deferred time is based on the type of update:</span></span>
    - <span data-ttu-id="d2ffb-110">การ**อัปเดตที่มีคุณภาพ**สามารถรอได้ถึง30วันจากการวางจำหน่ายของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="d2ffb-110">**Quality updates**  can be deferred up to 30 days from their release.</span></span>
    - <span data-ttu-id="d2ffb-111">การ**อัปเดตของฟีเจอร์**สามารถเลื่อนออกไปได้ถึง๑๘๐วันจากการวางจำหน่ายของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="d2ffb-111">**Feature updates**  can be deferred up to 180 days from their release.</span></span>
