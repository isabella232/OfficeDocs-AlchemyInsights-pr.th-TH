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
ms.openlocfilehash: 6a7c0497243ef7425917f54815e61f1244838c54
ms.sourcegitcommit: b14aa00b42ce4ca9d7dc3aa1fd57e66eae115447
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/28/2019
ms.locfileid: "30953363"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="7c084-102">จำกัดการ SharePoint แบบออนไลน์สำหรับโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="7c084-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="7c084-103">ยังคงบางองค์กรจำเป็นต้องมีประสบการณ์การใช้งานโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="7c084-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="7c084-104">ในขณะที่ไม่มีแผนการเอาโหมดคลาสสิกที่ระดับ granular เริ่มต้นเดือนเมษายน 1,2019 คุณจะไม่สามารถจำกัดทั้งองค์กร (ผู้เช่า) ไปยังโหมดคลาสสิกสำหรับรายการและไลบรารี</span><span class="sxs-lookup"><span data-stu-id="7c084-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="7c084-105">ผู้ดูแลจะมีตัวเลือกต่อไปนี้ในการจัดการแต่ละรายการและไลบรารีในโหมดคลาสสิกใช้สวิตช์เลือกเอาท์ granular ที่เราให้ในระดับดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7c084-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

<span data-ttu-id="7c084-106">ไลบรารี -ไซต์คอลเลกชัน -ไซต์ - รายการ--</span><span class="sxs-lookup"><span data-stu-id="7c084-106">-- site collection -- site -- list -- library</span></span>

<span data-ttu-id="7c084-107">นอกจากนี้ รายการที่ใช้คุณลักษณะบางอย่างและการกำหนดเองที่ไม่ได้รับการสนับสนุน โดยแบบสมัยใหม่จะยังคงสามารถจะสลับไปยังโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="7c084-107">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="7c084-108">หลังจากวันที่ 1 เมษายน รายการและไลบรารีที่อยู่ในโหมดคลาสสิกที่เป็นผลมาจากผู้เช่าเข้าร่วมออก จะโดยอัตโนมัติได้รับการจัดการที่ระดับไซต์และรายการระดับ</span><span class="sxs-lookup"><span data-stu-id="7c084-108">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="7c084-109">หากคุณต้องใช้โหมดคลาสสิก โปรดดูข้อมูลเพิ่มเติมที่นี่ และ PnP Powershell คำแนะนำที่นี่ที่อธิบายถึงตัวเลือกและเครื่องมือคุณสามารถใช้วันนี้เพื่อจัดเตรียมสำหรับการเอาออกการเช่าระดับเข้าร่วมออกในวันที่ 1 เมษายน</span><span class="sxs-lookup"><span data-stu-id="7c084-109">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
