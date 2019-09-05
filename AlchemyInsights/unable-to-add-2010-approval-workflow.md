---
title: ไม่สามารถเพิ่มลำดับงานการอนุมัติ๒๐๑๐
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748703"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="0f1d5-102">ไม่สามารถเพิ่มลำดับงานการอนุมัติ๒๐๑๐</span><span class="sxs-lookup"><span data-stu-id="0f1d5-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="0f1d5-103">ในไซต์คอลเลกชัน Microsoft SharePoint คุณไม่สามารถเพิ่มเวิร์กโฟลว์นำมาใช้ทั่วโลก (เช่น "การอนุมัติ SharePoint ๒๐๑๐") ไปยังรายการหรือไลบรารี</span><span class="sxs-lookup"><span data-stu-id="0f1d5-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="0f1d5-104">การแก้ไขปัญหานี้ให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="0f1d5-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="0f1d5-105">เปิดเว็บไซต์รากของไซต์คอลเลกชันใน SharePoint Designer ๒๐๑๓</span><span class="sxs-lookup"><span data-stu-id="0f1d5-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="0f1d5-106">ภายใต้**ไซต์วัตถุ**ให้เลือก**เวิร์กโฟลว์**</span><span class="sxs-lookup"><span data-stu-id="0f1d5-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="0f1d5-107">ในส่วน**ใหม่**ของ Ribbon ของ**เวิร์กโฟลว์**ให้เลือก**เวิร์กโฟลว์**ที่ใช้ซ้ำได้</span><span class="sxs-lookup"><span data-stu-id="0f1d5-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="0f1d5-108">ในแบบฟอร์ม**สร้างเวิร์กโฟลว์**ที่ใช้ซ้ำได้ให้ป้อนชื่อ \*\* *Repair2010* \*\*</span><span class="sxs-lookup"><span data-stu-id="0f1d5-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="0f1d5-109">สำหรับ**ชนิดแพลตฟอร์ม**คลิก**SharePoint ๒๐๑๐เวิร์กโฟลว์**และจากนั้นคลิ**กตกลง**</span><span class="sxs-lookup"><span data-stu-id="0f1d5-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="0f1d5-110">ในส่วน**บันทึก**ของ Ribbon ของ**เวิร์กโฟลว์**ให้เลือก**เผยแพร่**</span><span class="sxs-lookup"><span data-stu-id="0f1d5-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="0f1d5-111">ในส่วน**จัดการ**ของ Ribbon ของ**เวิร์กโฟลว์**ให้เลือก**เผยแพร่ทั่วโลก**</span><span class="sxs-lookup"><span data-stu-id="0f1d5-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="0f1d5-112">ในกล่องโต้ตอบการยืนยันที่ปรากฏขึ้นให้เลือก **' ตกลง '**</span><span class="sxs-lookup"><span data-stu-id="0f1d5-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="0f1d5-113">ในเว็บเบราว์เซอร์ค้นหาเว็บไซต์รากของไซต์คอลเลกชันและจากนั้นเข้าถึงลักษณะการทำงานของไซต์**คอลเลกชัน\*\*\*\*การตั้งค่า** \>ไซต์</span><span class="sxs-lookup"><span data-stu-id="0f1d5-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="0f1d5-114">สลับคุณลักษณะ**เวิร์กโฟลว์**:</span><span class="sxs-lookup"><span data-stu-id="0f1d5-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="0f1d5-115">· ถ้าคุณลักษณะถูก*เรียกใช้*งานให้คลิก**ปิด\*\*\*\*ใช้งาน**และจากนั้น</span><span class="sxs-lookup"><span data-stu-id="0f1d5-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="0f1d5-116">· ถ้า\*ปิด\***ใช้งาน**คุณลักษณะนี้แล้ว</span><span class="sxs-lookup"><span data-stu-id="0f1d5-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="0f1d5-117">สำหรับข้อมูลเพิ่มเติมโปรดดูที่[บทความ](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="0f1d5-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

