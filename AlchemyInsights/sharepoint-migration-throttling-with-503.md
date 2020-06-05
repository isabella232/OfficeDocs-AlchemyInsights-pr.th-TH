---
title: การควบคุมปริมาณการโยกย้าย SharePoint ที่ มีข้อผิดพลาด 503
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 3705be1e82fde6620fef3c4272f0294d58f11d38
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582902"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="d5d9d-102">การควบคุมปริมาณการโยกย้าย SharePoint ที่ มีข้อผิดพลาด 503</span><span class="sxs-lookup"><span data-stu-id="d5d9d-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="d5d9d-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้เรากําลังดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงมีอยู่มาก - โปรดเยี่ยมชม[SharePoint ออนไลน์ชั่วคราวการปรับปรุงคุณลักษณะ](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="d5d9d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d5d9d-104">**ข้อผิดพลาด 503 เมื่อย้ายข้อมูลไปยัง SharePoint แบบออนไลน์**</span><span class="sxs-lookup"><span data-stu-id="d5d9d-104">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="d5d9d-105">ปรากฏว่าคุณกําลังโยกย้ายไปยัง SharePoint Online และได้รับข้อผิดพลาด 503</span><span class="sxs-lookup"><span data-stu-id="d5d9d-105">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="d5d9d-106">โปรดทําตามขั้นตอนด้านล่างเพื่อให้เราอาจจะช่วยเหลือคุณโดยเร็วที่สุด</span><span class="sxs-lookup"><span data-stu-id="d5d9d-106">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="d5d9d-107">คลิก**ติดต่อฝ่ายสนับสนุน**แล้ว**สร้างคําขอบริการ**</span><span class="sxs-lookup"><span data-stu-id="d5d9d-107">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="d5d9d-108">สําหรับชื่อเรื่องและคําอธิบาย ให้พิมพ์**การควบคุมปริมาณการโยกย้าย SharePoint ด้วย 503**</span><span class="sxs-lookup"><span data-stu-id="d5d9d-108">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="d5d9d-109">เมื่อตั๋วถูกส่งแล้ว โปรดอัปเดตด้วยข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="d5d9d-109">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="d5d9d-110">เหลือการโยกย้าย (เช่น จํานวน TBs กี่คน)</span><span class="sxs-lookup"><span data-stu-id="d5d9d-110">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="d5d9d-111">วันที่เริ่มต้นและวันที่สิ้นสุดการย้าย</span><span class="sxs-lookup"><span data-stu-id="d5d9d-111">Migration start and end date.</span></span>
    - <span data-ttu-id="d5d9d-112">อธิบายตําแหน่งที่คุณกําลังย้ายเนื้อหาของคุณเช่น SharePoint Server, Box, GDrive, การแชร์ไฟล์ ฯลฯ</span><span class="sxs-lookup"><span data-stu-id="d5d9d-112">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="d5d9d-113">ประเมินจํานวนข้อผิดพลาดเกี่ยวกับการควบคุมปริมาณ (ตัวอย่างเช่น x เค้นต่อชั่วโมง?) และปริมาณการเกิดขึ้นเมื่อใด</span><span class="sxs-lookup"><span data-stu-id="d5d9d-113">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="d5d9d-114">เครื่องมือการโยกย้ายที่คุณใช้ (ตัวอย่างเช่น SPMT หรือ ShareGate)</span><span class="sxs-lookup"><span data-stu-id="d5d9d-114">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


