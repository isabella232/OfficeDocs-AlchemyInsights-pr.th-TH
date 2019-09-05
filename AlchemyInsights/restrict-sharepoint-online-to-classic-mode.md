---
title: จำกัด SharePoint แบบออนไลน์ไปยังโหมดคลาสสิก
ms.author: pebaum
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
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752087"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="d95a5-102">จำกัด SharePoint แบบออนไลน์ไปยังโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="d95a5-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="d95a5-103">บางองค์กรยังคงต้องการประสบการณ์ใช้งานโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="d95a5-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="d95a5-104">ในขณะที่ไม่มีแผนการลบโหมดคลาสสิกในระดับที่ละเอียดไม่สามารถจำกัดทั้งองค์กร (ผู้เช่า) ไปยังโหมดคลาสสิกสำหรับรายการและไลบรารีได้อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="d95a5-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="d95a5-105">ผู้ดูแลจะมีตัวเลือกต่อไปนี้ในการจัดการรายการและไลบรารีในโหมดคลาสสิกโดยใช้สวิตช์การเลือกที่เป็นเม็ดที่เราให้ไว้ในระดับต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="d95a5-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="d95a5-106">ชุดเก็บรวบรวมไซต์</span><span class="sxs-lookup"><span data-stu-id="d95a5-106">site collection</span></span>
- <span data-ttu-id="d95a5-107">ไซต์</span><span class="sxs-lookup"><span data-stu-id="d95a5-107">site</span></span>
- <span data-ttu-id="d95a5-108">รายการ</span><span class="sxs-lookup"><span data-stu-id="d95a5-108">list</span></span>
- <span data-ttu-id="d95a5-109">ไลบ รา รี</span><span class="sxs-lookup"><span data-stu-id="d95a5-109">library</span></span>

<span data-ttu-id="d95a5-110">นอกจากนี้รายการที่ใช้คุณลักษณะบางอย่างและการกำหนดเองที่ไม่ได้รับการสนับสนุนโดยแบบสมัยใหม่จะยังคงถูกสลับไปยังโหมดคลาสสิกโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="d95a5-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="d95a5-111">เริ่มต้นวันที่1เมษายน๒๐๑๙กระบวนการปิดใช้งานระดับผู้เช่าไม่เลือกจากรายการที่ทันสมัยและไลบรารีจะเริ่มต้นและดำเนินการต่อถึง31พฤษภาคม๒๐๑๙</span><span class="sxs-lookup"><span data-stu-id="d95a5-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="d95a5-112">รายการและไลบรารีที่อยู่ในโหมดคลาสสิกเป็นผลมาจากการเลือกไม่ใช้ผู้เช่าจะถูกเลื่อนไปทันสมัยโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="d95a5-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="d95a5-113">หากคุณต้องการโหมดคลาสสิกโปรดดูข้อมูลเพิ่มเติมที่[นี่](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)และคำแนะนำของ Powershell PnP ที่[นี่](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout)ซึ่งอธิบายถึงตัวเลือกและเครื่องมือที่คุณสามารถใช้ในวันนี้เพื่อใช้ประสบการณ์ในโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="d95a5-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
