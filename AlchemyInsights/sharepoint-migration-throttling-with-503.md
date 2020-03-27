---
title: การควบคุมปริมาณการโยกย้าย SharePoint ที่มีข้อผิดพลาด 503
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 05e816141a5b9cf484a647f8154110cd999ff6ef
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958701"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="6fd69-102">การควบคุมปริมาณการโยกย้าย SharePoint ที่มีข้อผิดพลาด 503</span><span class="sxs-lookup"><span data-stu-id="6fd69-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="6fd69-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="6fd69-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="6fd69-104">**ข้อผิดพลาด 503 เมื่อโยกย้ายไปยัง SharePoint แบบออนไลน์**</span><span class="sxs-lookup"><span data-stu-id="6fd69-104">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="6fd69-105">ดูเหมือนว่าคุณกําลังโยกย้ายไปยัง SharePoint Online และรับข้อผิดพลาด 503</span><span class="sxs-lookup"><span data-stu-id="6fd69-105">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="6fd69-106">โปรดทําตามขั้นตอนด้านล่างเพื่อให้เราสามารถช่วยคุณโดยเร็วที่สุด</span><span class="sxs-lookup"><span data-stu-id="6fd69-106">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="6fd69-107">คลิก**ติดต่อฝ่ายสนับสนุน**แล้วคลิก**คําขอบริการใหม่**</span><span class="sxs-lookup"><span data-stu-id="6fd69-107">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="6fd69-108">สําหรับชื่อเรื่องและคําอธิบาย ให้พิมพ์**การควบคุมปริมาณการย้าย SharePoint ด้วย 503**</span><span class="sxs-lookup"><span data-stu-id="6fd69-108">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="6fd69-109">เมื่อตั๋วถูกส่งไปแล้ว โปรดอัปเดตด้วยข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="6fd69-109">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="6fd69-110">จํานวนการโยกย้าย (เช่น จํานวน TBs)</span><span class="sxs-lookup"><span data-stu-id="6fd69-110">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="6fd69-111">วันที่เริ่มต้นและวันที่สิ้นสุดการโยกย้าย</span><span class="sxs-lookup"><span data-stu-id="6fd69-111">Migration start and end date.</span></span>
    - <span data-ttu-id="6fd69-112">อธิบายตําแหน่งที่คุณกําลังย้ายเนื้อหาของคุณ เช่น SharePoint Server, Box, GDrive, การแชร์ไฟล์ และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="6fd69-112">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="6fd69-113">ประมาณจํานวนข้อผิดพลาดการควบคุมปริมาณ (ตัวอย่างเช่น การควบคุมปริมาณ x ต่อชั่วโมง)และเมื่อการควบคุมปริมาณเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="6fd69-113">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="6fd69-114">เครื่องมือการโยกย้ายที่คุณกําลังใช้ (ตัวอย่างเช่น SPMT หรือ ShareGate)</span><span class="sxs-lookup"><span data-stu-id="6fd69-114">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


