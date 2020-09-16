---
title: จำกัด SharePoint Online เป็นโหมดคลาสสิก
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751442"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="3185e-102">จำกัด SharePoint Online เป็นโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="3185e-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="3185e-103">บางองค์กรยังจำเป็นต้องใช้ประสบการณ์การใช้งานโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="3185e-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="3185e-104">ในขณะที่ไม่มีแผนที่จะเอาโหมดคลาสสิกออกจากระดับที่เป็นเม็ดจะไม่สามารถจำกัดทั้งองค์กร (ผู้เช่า) เป็นโหมดคลาสสิกสำหรับรายการและไลบรารีได้อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="3185e-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="3185e-105">ผู้ดูแลระบบจะมีตัวเลือกต่อไปนี้ในการจัดการรายการและไลบรารีแต่ละรายการในโหมดคลาสสิกโดยใช้การสลับการเลือกแบบเม็ดที่เรามีให้ในระดับต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="3185e-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="3185e-106">ไซต์คอลเลกชัน</span><span class="sxs-lookup"><span data-stu-id="3185e-106">site collection</span></span>
- <span data-ttu-id="3185e-107">ไซต์</span><span class="sxs-lookup"><span data-stu-id="3185e-107">site</span></span>
- <span data-ttu-id="3185e-108">รายการ</span><span class="sxs-lookup"><span data-stu-id="3185e-108">list</span></span>
- <span data-ttu-id="3185e-109">ไลบ</span><span class="sxs-lookup"><span data-stu-id="3185e-109">library</span></span>

<span data-ttu-id="3185e-110">นอกจากนี้รายการที่ใช้บางฟีเจอร์และการกำหนดเองที่ไม่ได้รับการสนับสนุนโดยสมัยใหม่จะยังคงถูกสลับไปยังโหมดคลาสสิกโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="3185e-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="3185e-111">เริ่มต้นวันที่1เมษายน๒๐๑๙กระบวนการปิดใช้งานระดับผู้เช่าเลือกไม่อยู่ในรายการและไลบรารีที่ทันสมัยจะเริ่มต้นและดำเนินการต่อไปจนถึง31พฤษภาคม๒๐๑๙</span><span class="sxs-lookup"><span data-stu-id="3185e-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="3185e-112">รายการและไลบรารีที่อยู่ในโหมดคลาสสิกอันเป็นผลมาจากการปฏิเสธการเข้าร่วมของผู้เช่าจะถูกเลื่อนไปยังสมัยใหม่โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="3185e-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="3185e-113">ถ้าคุณจำเป็นต้องใช้โหมดคลาสสิกโปรดดูข้อมูลเพิ่มเติมที่ [นี่](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) และคำแนะนำในการใช้งาน PnP Powershell ที่ [นี่](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) ซึ่งจะอธิบายตัวเลือกและเครื่องมือที่คุณสามารถใช้ได้ในวันนี้เพื่อใช้ประสบการณ์การใช้งานโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="3185e-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
