---
title: การหยุดการปรับปรุงตามกําหนดการ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555992"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="67616-102">การหยุดการปรับปรุงตามกําหนดการ</span><span class="sxs-lookup"><span data-stu-id="67616-102">Pausing scheduled updates</span></span>

<span data-ttu-id="67616-103">เมื่อคําสั่งหยุดชั่วคราวถูกนําออกใช้</span><span class="sxs-lookup"><span data-stu-id="67616-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="67616-104">ด้วยเหตุนี้อุปกรณ์ของคุณอาจมี:</span><span class="sxs-lookup"><span data-stu-id="67616-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="67616-105">ติดตั้งการปรับปรุงตามกําหนดการก่อนเช็คอิน</span><span class="sxs-lookup"><span data-stu-id="67616-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="67616-106">ปิดการทํางานเมื่อคุณออกคําสั่งหยุดชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="67616-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="67616-107">ในกรณีนี้ เมื่ออุปกรณ์เปิดอยู่ อุปกรณ์เหล่านั้นอาจดาวน์โหลดและติดตั้งการปรับปรุงตามกําหนดการก่อนที่จะเช็คอิน</span><span class="sxs-lookup"><span data-stu-id="67616-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>