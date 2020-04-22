---
title: ไม่สามารถเรียกใช้เวิร์กโฟลว์ได้
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762120"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="c6c5a-102">ไม่สามารถเรียกใช้เวิร์กโฟลว์ได้</span><span class="sxs-lookup"><span data-stu-id="c6c5a-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="c6c5a-103">ในไซต์คอลเลกชัน Microsoft SharePoint คุณไม่สามารถเพิ่มเวิร์กโฟลว์ที่นํามาใช้ใหม่ได้แบบโกลบอล (เช่น "การอนุมัติ - SharePoint 2010") ลงในรายการหรือไลบรารี</span><span class="sxs-lookup"><span data-stu-id="c6c5a-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="c6c5a-104">เมื่อต้องการแก้ไขปัญหานี้ ให้ทําตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="c6c5a-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="c6c5a-105">เปิดเว็บไซต์รากของไซต์คอลเลกชันใน SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="c6c5a-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="c6c5a-106">ภายใต้**วัตถุของไซต์**ให้เลือก**เวิร์กโฟลว์**</span><span class="sxs-lookup"><span data-stu-id="c6c5a-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="c6c5a-107">ในส่วน**สร้าง**ของ Ribbon**เวิร์กโฟลว์**ให้เลือก**เวิร์กโฟลว์ที่นํามาใช้ใหม่**ได้</span><span class="sxs-lookup"><span data-stu-id="c6c5a-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="c6c5a-108">บน**แบบฟอร์มสร้างเวิร์กโฟลว์ที่นํามาใช้ใหม่**ได้ ให้ใส่ชื่อ \*\* *Repair2010* \*\*</span><span class="sxs-lookup"><span data-stu-id="c6c5a-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="c6c5a-109">สําหรับ**ชนิดแพลตฟอร์ม**ให้คลิก**เวิร์กโฟลว์ SharePoint 2010**แล้วคลิก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="c6c5a-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="c6c5a-110">ในส่วน**บันทึก**ของ Ribbon**เวิร์กโฟลว์**ให้เลือก**ประกาศ**</span><span class="sxs-lookup"><span data-stu-id="c6c5a-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="c6c5a-111">ในส่วน**จัดการ**ของ Ribbon**เวิร์กโฟลว์**ให้เลือก**เผยแพร่แบบรวม**</span><span class="sxs-lookup"><span data-stu-id="c6c5a-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="c6c5a-112">ในกล่องโต้ตอบการยืนยันที่ปรากฏ ให้เลือก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="c6c5a-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="c6c5a-113">ในเว็บเบราว์เซอร์ ให้ค้นหาตําแหน่งของเว็บไซต์รากของไซต์คอลเลกชัน แล้วเข้าถึง**คุณลักษณะไซต์คอลเลกชัน\*\*\*\*ของการตั้งค่าไซต์**\></span><span class="sxs-lookup"><span data-stu-id="c6c5a-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="c6c5a-114">จากนั้นสลับคุณลักษณะ**เวิร์กโฟลว์**:</span><span class="sxs-lookup"><span data-stu-id="c6c5a-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="c6c5a-115">· ถ้าลักษณะการทํางานเป็น*เรียกใช้*ให้คลิก**ปิดใช้งาน**แล้วคลิก**เปิดใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="c6c5a-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="c6c5a-116">· ถ้าปิดใช้งานลักษณะการทํางาน*ให้คลิก\*\*\*เรียกใช้*\*</span><span class="sxs-lookup"><span data-stu-id="c6c5a-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="c6c5a-117">สําหรับข้อมูลเพิ่มเติมโปรดดูที่[บทความ](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)ต่อไปนี้ของ</span><span class="sxs-lookup"><span data-stu-id="c6c5a-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

