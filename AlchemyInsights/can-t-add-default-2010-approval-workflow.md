---
title: ไม่สามารถเพิ่มค่าเริ่มต้นเวิร์กโฟลว์การอนุมัติ 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493041"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="50588-102">ไม่สามารถเพิ่มค่าเริ่มต้นเวิร์กโฟลว์การอนุมัติ 2010</span><span class="sxs-lookup"><span data-stu-id="50588-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="50588-103">ในคอลเลกชันของไซต์ Microsoft SharePoint คุณไม่สามารถเพิ่มเวิร์กโฟลว์สามารถแบบส่วนกลาง (เช่น "อนุมัติ - SharePoint 2010") รายการหรือไลบรารี</span><span class="sxs-lookup"><span data-stu-id="50588-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="50588-104">เมื่อต้องการแก้ไขปัญหานี้ ให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="50588-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="50588-105">เปิดเว็บไซต์รากของไซต์คอลเลกชันใน SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="50588-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="50588-106">ภายใต้**วัตถุไซต์**เลือก**ลำดับงาน**</span><span class="sxs-lookup"><span data-stu-id="50588-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="50588-107">ในส่วน**ใหม่**ของ ribbon**เวิร์กโฟลว์**เลือก**เวิร์กโฟลว์ Reusable**</span><span class="sxs-lookup"><span data-stu-id="50588-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="50588-p101">บนแบบฟอร์ม**สร้างเวิร์กโฟลว์ Reusable**ป้อนชื่อ \* **Repair2010**\* สำหรับ**ชนิดของแพลตฟอร์ม**เลือก**SharePoint 2010 โฟลว์**และจากนั้น ให้เลือก **'ตกลง'**</span><span class="sxs-lookup"><span data-stu-id="50588-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="50588-110">ในส่วน**บันทึก**ของ ribbon**เวิร์กโฟลว์**เลือก**เผยแพร่**</span><span class="sxs-lookup"><span data-stu-id="50588-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="50588-p102">ในส่วนการ**จัดการ**ของ ribbon**เวิร์กโฟลว์**เลือก**เผยแพร่แบบส่วนกลาง** ในกล่องโต้ตอบการยืนยันที่ปรากฏขึ้น เลือก **'ตกลง**'</span><span class="sxs-lookup"><span data-stu-id="50588-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="50588-p103">ในเว็บเบราว์เซอร์ ค้นหาเว็บไซต์รากของไซต์คอลเลกชัน และสามารถ เข้าถึง**การตั้งค่าไซต์** \> **คุณลักษณะของไซต์คอลเลกชัน** แล้วสลับไปยังลักษณะการทำงานของ**เวิร์กโฟลว์**:</span><span class="sxs-lookup"><span data-stu-id="50588-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="50588-115">· ถ้าคุณลักษณะนี้ถูก*เรียกใช้งานแล้ว*คลิก**เรียกใช้**และจากนั้น คลิก**เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="50588-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="50588-116">· ถ้าคุณลักษณะนี้ถูก*ปิดใช้งาน*คลิก**เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="50588-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="50588-117">สำหรับข้อมูลเพิ่มเติมโปรดดูที่[บท](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)ความต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="50588-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

