---
title: ไม่สามารถเพิ่มเวิร์กโฟลว์การอนุมัติ๒๐๑๐
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699754"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="8a9f6-102">ไม่สามารถเพิ่มเวิร์กโฟลว์การอนุมัติ๒๐๑๐</span><span class="sxs-lookup"><span data-stu-id="8a9f6-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="8a9f6-103">ในไซต์คอลเลกชันของ Microsoft SharePoint คุณจะไม่สามารถเพิ่มเวิร์กโฟลว์ที่นำกลับมาใช้ใหม่ได้ (เช่น "การอนุมัติ-SharePoint ๒๐๑๐") ลงในรายการหรือไลบรารี</span><span class="sxs-lookup"><span data-stu-id="8a9f6-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="8a9f6-104">เมื่อต้องการแก้ไขปัญหานี้ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="8a9f6-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="8a9f6-105">เปิดเว็บไซต์รากของไซต์คอลเลกชันใน SharePoint Designer ๒๐๑๓</span><span class="sxs-lookup"><span data-stu-id="8a9f6-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="8a9f6-106">ภายใต้**วัตถุของไซต์**ให้เลือก**เวิร์กโฟลว์**</span><span class="sxs-lookup"><span data-stu-id="8a9f6-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="8a9f6-107">ในส่วน **ใหม่** ของ Ribbon **เวิร์กโฟลว์** ให้เลือก **เวิร์กโฟลว์**ที่นำกลับมาใช้ใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="8a9f6-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="8a9f6-108">บนฟอร์ม **สร้างเวิร์กโฟลว์** ที่นำกลับมาใช้ใหม่ได้ให้ใส่ชื่อ \*\* *Repair2010* \*\*</span><span class="sxs-lookup"><span data-stu-id="8a9f6-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="8a9f6-109">สำหรับ**ชนิดของแพลตฟอร์ม**ให้คลิก**เวิร์กโฟลว์ SharePoint ๒๐๑๐**แล้วคลิก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="8a9f6-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="8a9f6-110">ในส่วน**บันทึก**ของ Ribbon**เวิร์กโฟลว์**ให้เลือก**เผยแพร่**</span><span class="sxs-lookup"><span data-stu-id="8a9f6-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="8a9f6-111">ในส่วน**จัดการ**ของ Ribbon**เวิร์กโฟลว์**ให้เลือก**เผยแพร่ทั่วโลก**</span><span class="sxs-lookup"><span data-stu-id="8a9f6-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="8a9f6-112">ในกล่องโต้ตอบการยืนยันที่ปรากฏขึ้นให้เลือก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="8a9f6-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="8a9f6-113">ในเว็บเบราว์เซอร์ให้ระบุตำแหน่งเว็บไซต์รากของไซต์คอลเลกชันแล้ว**เข้าถึง** \> **ฟีเจอร์ไซต์คอลเลกชันของไซต์คอลเลกชัน**</span><span class="sxs-lookup"><span data-stu-id="8a9f6-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="8a9f6-114">สลับลักษณะการทำงานของ **เวิร์กโฟลว์** :</span><span class="sxs-lookup"><span data-stu-id="8a9f6-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="8a9f6-115">· ถ้ามีการ*เปิด*ใช้งานฟีเจอร์แล้วให้คลิก**ปิด**ใช้งานแล้วคลิก**เปิดใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="8a9f6-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="8a9f6-116">· ถ้าฟีเจอร์ถูก*ปิด*ใช้งานให้คลิก**เปิดใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="8a9f6-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="8a9f6-117">สำหรับข้อมูลเพิ่มเติมโปรดดู [บทความ](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="8a9f6-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

