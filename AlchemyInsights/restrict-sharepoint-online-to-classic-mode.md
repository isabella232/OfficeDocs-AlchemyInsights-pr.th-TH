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
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 21cfb213183188d32a3743f66db10a8463019965
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/28/2019
ms.locfileid: "30956025"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="5ffa2-102">จำกัดการ SharePoint แบบออนไลน์สำหรับโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="5ffa2-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="5ffa2-103">ยังคงบางองค์กรจำเป็นต้องมีประสบการณ์การใช้งานโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="5ffa2-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="5ffa2-104">ในขณะที่ไม่มีแผนการเอาโหมดคลาสสิกที่ระดับ granular เริ่มต้นเดือนเมษายน 1,2019 คุณจะไม่สามารถจำกัดทั้งองค์กร (ผู้เช่า) ไปยังโหมดคลาสสิกสำหรับรายการและไลบรารี</span><span class="sxs-lookup"><span data-stu-id="5ffa2-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="5ffa2-105">ผู้ดูแลจะมีตัวเลือกต่อไปนี้ในการจัดการแต่ละรายการและไลบรารีในโหมดคลาสสิกใช้สวิตช์เลือกเอาท์ granular ที่เราให้ในระดับดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="5ffa2-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="5ffa2-106">ไซต์คอลเลกชัน</span><span class="sxs-lookup"><span data-stu-id="5ffa2-106">site collection</span></span>
- <span data-ttu-id="5ffa2-107">ไซต์</span><span class="sxs-lookup"><span data-stu-id="5ffa2-107">site</span></span>
- <span data-ttu-id="5ffa2-108">รายการ</span><span class="sxs-lookup"><span data-stu-id="5ffa2-108">list</span></span>
- <span data-ttu-id="5ffa2-109">ไลบรารี</span><span class="sxs-lookup"><span data-stu-id="5ffa2-109">library</span></span>

<span data-ttu-id="5ffa2-110">นอกจากนี้ รายการที่ใช้คุณลักษณะบางอย่างและการกำหนดเองที่ไม่ได้รับการสนับสนุน โดยแบบสมัยใหม่จะยังคงสามารถจะสลับไปยังโหมดคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="5ffa2-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="5ffa2-111">หลังจากวันที่ 1 เมษายน รายการและไลบรารีที่อยู่ในโหมดคลาสสิกที่เป็นผลมาจากผู้เช่าเข้าร่วมออก จะโดยอัตโนมัติได้รับการจัดการที่ระดับไซต์และรายการระดับ</span><span class="sxs-lookup"><span data-stu-id="5ffa2-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="5ffa2-112">หากคุณต้องใช้โหมดคลาสสิก โปรดดูข้อมูลเพิ่มเติมที่นี่ และ PnP Powershell คำแนะนำที่นี่ที่อธิบายถึงตัวเลือกและเครื่องมือคุณสามารถใช้วันนี้เพื่อจัดเตรียมสำหรับการเอาออกการเช่าระดับเข้าร่วมออกในวันที่ 1 เมษายน</span><span class="sxs-lookup"><span data-stu-id="5ffa2-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
