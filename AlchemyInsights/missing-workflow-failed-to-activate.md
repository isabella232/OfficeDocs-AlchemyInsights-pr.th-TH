---
title: ไม่สามารถเรียกใช้ลำดับงานที่ขาดหายไป
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052632"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="2bbcc-102">ไม่สามารถเรียกใช้ลำดับงานที่ขาดหายไป</span><span class="sxs-lookup"><span data-stu-id="2bbcc-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="2bbcc-103">ในไซต์คอลเลกชัน Microsoft SharePoint คุณไม่สามารถเพิ่มเวิร์กโฟลว์นำมาใช้ทั่วโลก (เช่น "การอนุมัติ SharePoint ๒๐๑๐") ไปยังรายการหรือไลบรารี</span><span class="sxs-lookup"><span data-stu-id="2bbcc-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="2bbcc-104">การแก้ไขปัญหานี้ให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="2bbcc-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="2bbcc-105">เปิดเว็บไซต์รากของไซต์คอลเลกชันใน SharePoint Designer ๒๐๑๓</span><span class="sxs-lookup"><span data-stu-id="2bbcc-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="2bbcc-106">ภายใต้**ไซต์วัตถุ**ให้เลือก**เวิร์กโฟลว์**</span><span class="sxs-lookup"><span data-stu-id="2bbcc-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="2bbcc-107">ในส่วน**ใหม่**ของ Ribbon ของ**เวิร์กโฟลว์**ให้เลือก**เวิร์กโฟลว์**ที่ใช้ซ้ำได้</span><span class="sxs-lookup"><span data-stu-id="2bbcc-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="2bbcc-108">ในแบบฟอร์ม**สร้างเวิร์กโฟลว์**ที่ใช้ซ้ำได้ให้ป้อนชื่อ \*\* *Repair2010* \*\*</span><span class="sxs-lookup"><span data-stu-id="2bbcc-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="2bbcc-109">สำหรับ**ชนิดแพลตฟอร์ม**คลิก**SharePoint ๒๐๑๐เวิร์กโฟลว์**และจากนั้นคลิ**กตกลง**</span><span class="sxs-lookup"><span data-stu-id="2bbcc-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="2bbcc-110">ในส่วน**บันทึก**ของ Ribbon ของ**เวิร์กโฟลว์**ให้เลือก**เผยแพร่**</span><span class="sxs-lookup"><span data-stu-id="2bbcc-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="2bbcc-111">ในส่วน**จัดการ**ของ Ribbon ของ**เวิร์กโฟลว์**ให้เลือก**เผยแพร่ทั่วโลก**</span><span class="sxs-lookup"><span data-stu-id="2bbcc-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="2bbcc-112">ในกล่องโต้ตอบการยืนยันที่ปรากฏขึ้นให้เลือก **' ตกลง '**</span><span class="sxs-lookup"><span data-stu-id="2bbcc-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="2bbcc-113">ในเว็บเบราว์เซอร์ค้นหาเว็บไซต์รากของไซต์คอลเลกชันและจากนั้นเข้าถึงลักษณะการทำงานของไซต์**คอลเลกชัน\*\*\*\*การตั้งค่า** \>ไซต์</span><span class="sxs-lookup"><span data-stu-id="2bbcc-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="2bbcc-114">สลับคุณลักษณะ**เวิร์กโฟลว์**:</span><span class="sxs-lookup"><span data-stu-id="2bbcc-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="2bbcc-115">· ถ้าคุณลักษณะถูก*เรียกใช้*งานให้คลิก**ปิด\*\*\*\*ใช้งาน**และจากนั้น</span><span class="sxs-lookup"><span data-stu-id="2bbcc-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="2bbcc-116">· ถ้า\*ปิด\***ใช้งาน**คุณลักษณะนี้แล้ว</span><span class="sxs-lookup"><span data-stu-id="2bbcc-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="2bbcc-117">สำหรับข้อมูลเพิ่มเติมโปรดดูที่[บทความ](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="2bbcc-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

