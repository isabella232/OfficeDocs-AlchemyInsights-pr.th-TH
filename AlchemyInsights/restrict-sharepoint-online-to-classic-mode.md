---
title: จํากัด SharePoint แบบออนไลน์เป็นโหมดคลาสสิก
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742488"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="8050c-102">จํากัด SharePoint แบบออนไลน์เป็นโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="8050c-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="8050c-103">บางองค์กรยังคงต้องการประสบการณ์การใช้งานโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="8050c-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="8050c-104">ในขณะที่ไม่มีแผนที่จะเอาโหมดคลาสสิกในระดับระดับย่อย, มันเป็นไปไม่ได้ที่จะ จํากัด ทั้งองค์กร (ผู้เช่า) ไปยังโหมดคลาสสิกสําหรับรายการและห้องสมุด.</span><span class="sxs-lookup"><span data-stu-id="8050c-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="8050c-105">ผู้ดูแลระบบจะมีตัวเลือกต่อไปนี้ในการจัดการรายการและไลบรารีแต่ละรายการในโหมดคลาสสิกโดยใช้สวิตช์เลือกออกแบบละเอียดที่เราให้อยู่ในระดับต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="8050c-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="8050c-106">ไซต์คอลเลกชัน</span><span class="sxs-lookup"><span data-stu-id="8050c-106">site collection</span></span>
- <span data-ttu-id="8050c-107">ไซต์</span><span class="sxs-lookup"><span data-stu-id="8050c-107">site</span></span>
- <span data-ttu-id="8050c-108">รายการ</span><span class="sxs-lookup"><span data-stu-id="8050c-108">list</span></span>
- <span data-ttu-id="8050c-109">ไลบ รา รี</span><span class="sxs-lookup"><span data-stu-id="8050c-109">library</span></span>

<span data-ttu-id="8050c-110">นอกจากนี้ รายการที่ใช้คุณลักษณะบางอย่างและการกําหนดค่าเองที่ไม่ได้รับการสนับสนุนโดยสมัยใหม่จะยังคงถูกสลับไปยังโหมดคลาสสิกโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="8050c-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="8050c-111">เริ่มต้น 1 เมษายน 2019 กระบวนการปิดการใช้งานระดับผู้เช่าเลือกออกจากรายการและไลบรารีที่ทันสมัยจะเริ่มต้น และดําเนินต่อถึง 31 พฤษภาคม 2019</span><span class="sxs-lookup"><span data-stu-id="8050c-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="8050c-112">รายการและไลบรารีที่อยู่ในโหมดคลาสสิกเนื่องจากผู้ใช้ผู้เช่าไม่รับจะถูกเลื่อนไปยังที่ทันสมัยโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="8050c-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="8050c-113">หากคุณต้องการโหมดคลาสสิกโปรดดูข้อมูลเพิ่มเติม[ที่นี่](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)และการเรียนการสอน Powershell PnP[ที่นี่](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout)ที่อธิบายตัวเลือกและเครื่องมือที่คุณสามารถใช้ในวันนี้เพื่อใช้ประสบการณ์โหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="8050c-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
