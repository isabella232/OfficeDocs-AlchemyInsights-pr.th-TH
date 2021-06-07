---
title: ปัญหาด้านประสิทธิภาพการ Microsoft Defender for Endpoint บน Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794224"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="74e5d-102">ปัญหาด้านประสิทธิภาพการ Microsoft Defender for Endpoint บน Linux</span><span class="sxs-lookup"><span data-stu-id="74e5d-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="74e5d-103">บทความนี้จะแนะแนวคุณผ่านขั้นตอนในการระบุปัญหาด้านประสิทธิภาพการแต่ละอย่างของ Microsoft Defender for Endpoint บน Linux</span><span class="sxs-lookup"><span data-stu-id="74e5d-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="74e5d-104">สิ่งสําคัญคือต้องตรวจสอบก่อนว่าปัญหาที่คุณพบได้รับการแก้ไขด้วย[เวอร์ชันล่าสุด](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="74e5d-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="74e5d-105">เมื่อต้องการเริ่มการตรวจสอบ ให้ดู แก้ไขปัญหา[ประสิทธิภาพการโยกย้าย Microsoft Defender for Endpoint บน Linux](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="74e5d-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="74e5d-106">การยกเว้น</span><span class="sxs-lookup"><span data-stu-id="74e5d-106">Exclusions</span></span>

<span data-ttu-id="74e5d-107">การยกเว้นสามารถช่วยบรรเทาปัญหาด้านประสิทธิภาพการช่วยได้</span><span class="sxs-lookup"><span data-stu-id="74e5d-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="74e5d-108">ตรวจสอบข้อยกเว้นของคุณก่อนที่คุณจะเริ่มต้น เพื่อให้ทราบและทราบความเสี่ยงเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="74e5d-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="74e5d-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="74e5d-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="74e5d-110">เมื่อคุณมีหลายไฟล์&โฟลเดอร์ที่ไม่ต้องการและทั้งหมดอยู่ในที่ยึดเดียวกัน การยกเว้นที่ยึดอาจง่ายกว่า</span><span class="sxs-lookup"><span data-stu-id="74e5d-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="74e5d-111">เริ่มต้นด้วยรุ่นเดือนกุมภาพันธ์ 101.22.80 คุณไม่สามารถยกเว้นจุดยึดทั้งหมดได้</span><span class="sxs-lookup"><span data-stu-id="74e5d-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="74e5d-112">ตัวอย่างเช่น ถ้า /mnt/backup เป็น mountpoint คุณสามารถเพิ่ม /mnt/backup ลงในรายการแยกโดยการเรียกใช้การสั่งนี้:</span><span class="sxs-lookup"><span data-stu-id="74e5d-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="74e5d-113">**หมายเหตุ**: การเพิ่มการยกเว้นจะมีความเสี่ยงต่อมัลแวร์ที่จะไม่ถูกตรวจพบและควรได้รับการจัดการและดําเนินการด้วยความระมัดระวัง</span><span class="sxs-lookup"><span data-stu-id="74e5d-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="74e5d-114">ต้องการความช่วยเหลือหรือไม่</span><span class="sxs-lookup"><span data-stu-id="74e5d-114">Need Help?</span></span>

<span data-ttu-id="74e5d-115">เพื่อช่วยคุณอย่างมีประสิทธิภาพสูงสุด ให้รวบรวมข้อมูลการวินิจฉัยก่อนที่จะเปิดกรณีสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="74e5d-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
