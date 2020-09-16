---
title: การโยกย้าย SharePoint ที่มีข้อผิดพลาด๕๐๓
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: e46c39652db6a13a45d77d303102b4873e67a076
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720080"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="c46c2-102">การโยกย้าย SharePoint ที่มีข้อผิดพลาด๕๐๓</span><span class="sxs-lookup"><span data-stu-id="c46c2-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="c46c2-103">**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="c46c2-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c46c2-104">**ข้อผิดพลาด๕๐๓เมื่อโยกย้ายไปยัง SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="c46c2-104">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="c46c2-105">แสดงว่าคุณกำลังโยกย้ายไปยัง SharePoint Online และได้รับข้อผิดพลาด๕๐๓</span><span class="sxs-lookup"><span data-stu-id="c46c2-105">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="c46c2-106">โปรดทำตามขั้นตอนด้านล่างเพื่อให้เราสามารถช่วยคุณได้โดยเร็วที่สุดเท่าที่จะเป็นไปได้</span><span class="sxs-lookup"><span data-stu-id="c46c2-106">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="c46c2-107">คลิก**ติดต่อฝ่ายสนับสนุน**แล้วคลิก**คำขอบริการใหม่**</span><span class="sxs-lookup"><span data-stu-id="c46c2-107">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="c46c2-108">สำหรับชื่อเรื่องและคำอธิบายให้พิมพ์การ**โยกย้าย SharePoint ที่ควบคุมปริมาณด้วย๕๐๓**</span><span class="sxs-lookup"><span data-stu-id="c46c2-108">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="c46c2-109">เมื่อมีการส่งตั๋วแล้วโปรดอัปเดตข้อมูลดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="c46c2-109">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="c46c2-110">จำนวนครั้งที่เหลือของการโยกย้าย (ตัวอย่างเช่นกี่ช้อนโต๊ะ)</span><span class="sxs-lookup"><span data-stu-id="c46c2-110">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="c46c2-111">วันที่เริ่มต้นและวันที่สิ้นสุดการโยกย้าย</span><span class="sxs-lookup"><span data-stu-id="c46c2-111">Migration start and end date.</span></span>
    - <span data-ttu-id="c46c2-112">อธิบายว่าคุณกำลังโยกย้ายเนื้อหาของคุณจากที่ใดเช่น SharePoint Server กล่อง GDrive การแชร์ไฟล์และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="c46c2-112">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="c46c2-113">ประเมินจำนวนข้อผิดพลาดในการควบคุมปริมาณ (ตัวอย่างเช่น x throttle ต่อชั่วโมงหรือไม่) และเมื่อใดที่การควบคุมปริมาณเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="c46c2-113">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="c46c2-114">เครื่องมือการโยกย้ายแบบใดที่คุณกำลังใช้ (ตัวอย่างเช่น SPMT หรือ ShareGate)</span><span class="sxs-lookup"><span data-stu-id="c46c2-114">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


