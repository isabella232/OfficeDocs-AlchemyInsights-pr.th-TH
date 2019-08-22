---
title: ขาดลำดับงานไม่สามารถเปิดใช้งาน
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 44fd3c2d1e8b278b47c0fde6d48c7cbcbaa5c324
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543944"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="9df62-102">ขาดลำดับงานไม่สามารถเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="9df62-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="9df62-103">ในคอลเลกชันของไซต์ Microsoft SharePoint คุณไม่สามารถเพิ่มเวิร์กโฟลว์สามารถแบบส่วนกลาง (เช่น "อนุมัติ - SharePoint 2010") รายการหรือไลบรารี</span><span class="sxs-lookup"><span data-stu-id="9df62-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="9df62-104">เมื่อต้องการแก้ไขปัญหานี้ ให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="9df62-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="9df62-105">เปิดเว็บไซต์รากของไซต์คอลเลกชันใน SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="9df62-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="9df62-106">ภายใต้**วัตถุไซต์**เลือก**ลำดับงาน**</span><span class="sxs-lookup"><span data-stu-id="9df62-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="9df62-107">ในส่วน**ใหม่**ของ ribbon**เวิร์กโฟลว์**เลือก**เวิร์กโฟลว์ Reusable**</span><span class="sxs-lookup"><span data-stu-id="9df62-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="9df62-108">บนแบบฟอร์ม**สร้างเวิร์กโฟลว์ Reusable**ป้อนชื่อ \*\* *Repair2010* \*\*</span><span class="sxs-lookup"><span data-stu-id="9df62-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="9df62-109">สำหรับ**ชนิดของแพลตฟอร์ม\*\*\*\*เวิร์กโฟลว์ 2010 SharePoint**คลิก และจากนั้น คลิก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="9df62-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="9df62-110">ในส่วน**บันทึก**ของ ribbon**เวิร์กโฟลว์**เลือก**เผยแพร่**</span><span class="sxs-lookup"><span data-stu-id="9df62-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="9df62-111">ในส่วนการ**จัดการ**ของ ribbon**เวิร์กโฟลว์**เลือก**เผยแพร่แบบส่วนกลาง**</span><span class="sxs-lookup"><span data-stu-id="9df62-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="9df62-112">ในกล่องโต้ตอบการยืนยันที่ปรากฏขึ้น เลือก **'ตกลง**'</span><span class="sxs-lookup"><span data-stu-id="9df62-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="9df62-113">ในเว็บเบราว์เซอร์ ค้นหาเว็บไซต์รากของไซต์คอลเลกชัน และสามารถ เข้าถึง**การตั้งค่าไซต์** \> **คุณลักษณะของไซต์คอลเลกชัน**</span><span class="sxs-lookup"><span data-stu-id="9df62-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="9df62-114">แล้วสลับไปยังลักษณะการทำงานของ**เวิร์กโฟลว์**:</span><span class="sxs-lookup"><span data-stu-id="9df62-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="9df62-115">· ถ้าคุณลักษณะนี้ถูก*เรียกใช้งานแล้ว*คลิก**เรียกใช้**และจากนั้น คลิก**เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="9df62-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="9df62-116">· ถ้าคุณลักษณะนี้ถูก*ปิดใช้งาน*คลิก**เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="9df62-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="9df62-117">สำหรับข้อมูลเพิ่มเติมโปรดดูที่[บท](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)ความต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="9df62-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

