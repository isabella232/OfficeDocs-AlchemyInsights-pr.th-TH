---
title: แก้ไขปัญหาการใช้เปิดด้วย Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659077"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="31156-102">แก้ไขปัญหาเกี่ยวกับการเปิดด้วย Explorer</span><span class="sxs-lookup"><span data-stu-id="31156-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="31156-103">แก้ไขปัญหาทั่วไปเกี่ยวกับการเปิดไลบรารีเอกสารใน SharePoint หรือ OneDrive โดยใช้คำสั่ง **เปิดด้วย Explorer** :</span><span class="sxs-lookup"><span data-stu-id="31156-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="31156-104">ใช้ Internet Explorer 10 หรือ Internet Explorer 11</span><span class="sxs-lookup"><span data-stu-id="31156-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="31156-105">**เปิดด้วย Explorer** ไม่เข้ากันได้กับ Microsoft Edge, Google Chrome, Firefox และผู้อื่น</span><span class="sxs-lookup"><span data-stu-id="31156-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="31156-106">**เปิดด้วย Explorer** ถูกปิดใช้งานในเบราว์เซอร์ทั้งหมดยกเว้น Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="31156-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="31156-107">**เปิดด้วย Explorer** ไม่พร้อมใช้งานในประสบการณ์การใช้งานที่ทันสมัยสำหรับไลบรารี SharePoint</span><span class="sxs-lookup"><span data-stu-id="31156-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="31156-108">ใช้ **มุมมองใน File Explorer** แทน</span><span class="sxs-lookup"><span data-stu-id="31156-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="31156-109">เลือกมุมมอง**ตัวเลือกมุมมอง** \> **ใน File Explorer**</span><span class="sxs-lookup"><span data-stu-id="31156-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="31156-110">ดูใน File Explorer ไม่เข้ากันกับ Microsoft Edge, Google Chrome, Firefox และผู้อื่น</span><span class="sxs-lookup"><span data-stu-id="31156-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="31156-111">**ดูใน File explorer** ที่พร้อมใช้งานเฉพาะใน Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="31156-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="31156-112">ตรวจสอบให้แน่ใจว่าบริการ WebClient กำลังทำงานอยู่</span><span class="sxs-lookup"><span data-stu-id="31156-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="31156-113">ในกล่องค้นหาของ Windows ให้พิมพ์เรียกใช้เลือกแอปเรียกใช้เดสก์ท็อปพิมพ์ services. msc แล้วกด Enter</span><span class="sxs-lookup"><span data-stu-id="31156-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="31156-114">เลื่อนลงไปยังบริการ WebClient และตรวจสอบให้แน่ใจว่าคอลัมน์ **สถานะ** แสดง "กำลังทำงาน"</span><span class="sxs-lookup"><span data-stu-id="31156-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="31156-115">ถ้าไม่ใช่ให้ดับเบิลคลิกที่บริการนั้นแล้วคลิก**เริ่ม**แล้วคลิก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="31156-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="31156-116">(คุณอาจจำเป็นต้องเปิดใช้งานบริการก่อนด้วยการเลือก **ด้วยตนเอง** หรือ **โดยอัตโนมัติ** ในกล่อง **ชนิดการเริ่มต้น** )</span><span class="sxs-lookup"><span data-stu-id="31156-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="31156-117">การเปิดไลบรารีใน File Explorer มีประโยชน์ในกรณีที่คุณต้องการคัดลอกหรือย้ายไฟล์และโฟลเดอร์หลายๆไฟล์แต่ถ้าคุณต้องการทำงานในไลบรารีเป็นประจำเราขอแนะนำให้ซิงค์</span><span class="sxs-lookup"><span data-stu-id="31156-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="31156-118">เมื่อต้องการแก้ไขปัญหาการเปิดใน File Explorer ให้ดูที่[เปิดใน Explorer](https://go.microsoft.com/fwlink/?linkid=871665)</span><span class="sxs-lookup"><span data-stu-id="31156-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="31156-119">สำหรับข้อมูลเกี่ยวกับการตั้งค่าการซิงค์ให้ดู[ที่ซิงค์ไฟล์ SharePoint ด้วยไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://go.microsoft.com/fwlink/?linkid=871666)</span><span class="sxs-lookup"><span data-stu-id="31156-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="31156-120">โปรดดูบทความ [วิธีใช้คำสั่ง "เปิดด้วย Explorer" เพื่อแก้ไขปัญหาใน SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="31156-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

