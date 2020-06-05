---
title: ไม่สามารถเพิ่มเวิร์กโฟลว์การอนุมัติ 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582866"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="7da13-102">ไม่สามารถเพิ่มเวิร์กโฟลว์การอนุมัติ 2010</span><span class="sxs-lookup"><span data-stu-id="7da13-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="7da13-103">ในไซต์คอลเลกชัน Microsoft SharePoint คุณไม่สามารถเพิ่มเวิร์กโฟลว์ที่นํากลับมาใช้ใหม่ได้แบบส่วนกลาง (เช่น "อนุมัติ - SharePoint 2010") ลงในรายการหรือไลบรารี</span><span class="sxs-lookup"><span data-stu-id="7da13-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="7da13-104">เมื่อต้องการแก้ไขปัญหานี้ ให้ทําตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="7da13-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="7da13-105">เปิดเว็บไซต์รากของไซต์คอลเลกชันใน SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="7da13-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="7da13-106">ภายใต้**วัตถุไซต์**ให้เลือก**เวิร์กโฟลว์**</span><span class="sxs-lookup"><span data-stu-id="7da13-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="7da13-107">ในส่วน**สร้าง**ของ Ribbon**เวิร์กโฟลว์**ให้เลือก**เวิร์กโฟลว์ที่นํากลับมาใช้ใหม่ได้**</span><span class="sxs-lookup"><span data-stu-id="7da13-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="7da13-108">บนแบบฟอร์ม**สร้างเวิร์กโฟลว์ที่นํากลับมาใช้ใหม่**ได้ ให้ป้อนชื่อ \*\* *Repair2010* \*\*</span><span class="sxs-lookup"><span data-stu-id="7da13-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="7da13-109">สําหรับ**ชนิดแพลตฟอร์ม**ให้คลิก**เวิร์กโฟลว์ SharePoint 2010**แล้วคลิก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="7da13-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="7da13-110">ในส่วน**บันทึก**ของ Ribbon**เวิร์กโฟลว์**ให้เลือก**เผยแพร่**</span><span class="sxs-lookup"><span data-stu-id="7da13-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="7da13-111">ในส่วน**จัดการ**ของ Ribbon**เวิร์กโฟลว์**ให้เลือก**เผยแพร่ส่วนกลาง**</span><span class="sxs-lookup"><span data-stu-id="7da13-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="7da13-112">ในกล่องโต้ตอบการยืนยันที่ปรากฏขึ้น ให้เลือก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="7da13-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="7da13-113">ในเว็บเบราว์เซอร์ ให้ค้นหาเว็บไซต์รากของไซต์คอลเลกชัน จากนั้นเข้าถึง**Site Settings** \> **คุณลักษณะไซต์คอลเลกชันการตั้งค่าไซต์**</span><span class="sxs-lookup"><span data-stu-id="7da13-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="7da13-114">สลับคุณลักษณะ**เวิร์กโฟลว์**:</span><span class="sxs-lookup"><span data-stu-id="7da13-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="7da13-115">· ถ้า*ลักษณะการทํางานเปิดใช้งานแล้ว*ให้คลิก**ปิดใช้งาน**แล้วคลิก**เปิดใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="7da13-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="7da13-116">· ถ้าลักษณะการทํางาน*ถูกปิดใช้งาน*ให้คลิก**เปิดใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="7da13-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="7da13-117">สําหรับข้อมูลเพิ่มเติมโปรดดูที่[บทความ](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="7da13-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

