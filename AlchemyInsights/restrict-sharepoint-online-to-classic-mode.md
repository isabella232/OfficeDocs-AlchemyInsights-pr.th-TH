---
title: จำกัดการ SharePoint แบบออนไลน์สำหรับโหมดคลาสสิก
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: e7ecfd8c2f1a532355bfb8c2c0a846fc0d6e88b1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551578"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="153dd-102">จำกัดการ SharePoint แบบออนไลน์สำหรับโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="153dd-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="153dd-103">ยังคงบางองค์กรจำเป็นต้องมีประสบการณ์การใช้งานโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="153dd-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="153dd-104">ในขณะที่ไม่มีแผนการเอาโหมดคลาสสิกที่ระดับ granular จะไม่สามารถจำกัดทั้งองค์กร (ผู้เช่า) ถึงโหมดคลาสสิกสำหรับรายการและไลบรารี</span><span class="sxs-lookup"><span data-stu-id="153dd-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="153dd-105">ผู้ดูแลจะมีตัวเลือกต่อไปนี้ในการจัดการแต่ละรายการและไลบรารีในโหมดคลาสสิกใช้สวิตช์เลือกเอาท์ granular ที่เราให้ในระดับดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="153dd-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="153dd-106">ไซต์คอลเลกชัน</span><span class="sxs-lookup"><span data-stu-id="153dd-106">site collection</span></span>
- <span data-ttu-id="153dd-107">ไซต์</span><span class="sxs-lookup"><span data-stu-id="153dd-107">site</span></span>
- <span data-ttu-id="153dd-108">รายการ</span><span class="sxs-lookup"><span data-stu-id="153dd-108">list</span></span>
- <span data-ttu-id="153dd-109">ไลบรารี</span><span class="sxs-lookup"><span data-stu-id="153dd-109">library</span></span>

<span data-ttu-id="153dd-110">นอกจากนี้ รายการที่ใช้คุณลักษณะบางอย่างและการกำหนดเองที่ไม่ได้รับการสนับสนุน โดยแบบสมัยใหม่จะยังคงสามารถจะสลับไปยังโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="153dd-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="153dd-111">เริ่มต้นเดือน 1 เมษายน 2019 กระบวนการปิดการใช้งานระดับผู้เช่าเลือกออกจากรายการสมัยใหม่ และไลบรารีจะเริ่มการทำงาน และดำเนินต่อผ่าน 31 พฤษภาคม 2019</span><span class="sxs-lookup"><span data-stu-id="153dd-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="153dd-112">รายการและไลบรารีที่อยู่ในโหมดคลาสสิกที่เป็นผลมาจากผู้เช่าเข้าร่วมออก จะโดยอัตโนมัติเลื่อนขึ้นไปสมัยใหม่</span><span class="sxs-lookup"><span data-stu-id="153dd-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="153dd-113">หากคุณต้องใช้โหมดคลาสสิกโปรดดูข้อมูลเพิ่มเติม[ที่นี่](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)และคำสั่ง PnP Powershell[ที่นี่](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout)ซึ่งอธิบายถึงตัวเลือกและเครื่องมือที่คุณสามารถใช้วันนี้เพื่อใช้กับประสบการณ์ใช้งานโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="153dd-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
