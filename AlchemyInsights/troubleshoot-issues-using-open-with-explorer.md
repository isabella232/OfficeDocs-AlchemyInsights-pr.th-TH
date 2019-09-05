---
title: การแก้ไขปัญหาโดยใช้เปิดด้วย Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742752"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="f6bf5-102">แก้ไขปัญหาเกี่ยวกับการเปิดด้วย Explorer</span><span class="sxs-lookup"><span data-stu-id="f6bf5-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="f6bf5-103">แก้ไขปัญหาทั่วไปเกี่ยวกับการเปิดไลบรารีเอกสารใน SharePoint หรือ OneDrive โดยใช้คำสั่ง**Open ด้วย Explorer** :</span><span class="sxs-lookup"><span data-stu-id="f6bf5-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="f6bf5-104">ใช้ Internet Explorer 10 หรือ 11 Explorer อินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="f6bf5-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="f6bf5-105">**เปิดด้วย Explorer**ไม่สามารถทำงานร่วมกับ Microsoft Edge, Google Chrome, Firefox และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="f6bf5-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="f6bf5-106">**เปิดด้วย Explorer**ถูกปิดใช้งานในเบราว์เซอร์ทั้งหมดยกเว้น Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="f6bf5-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="f6bf5-107">**เปิดด้วย Explorer**ไม่พร้อมใช้งานในประสบการณ์ที่ทันสมัยสำหรับไลบรารี SharePoint</span><span class="sxs-lookup"><span data-stu-id="f6bf5-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="f6bf5-108">ใช้**มุมมองใน File Explorer**แทน</span><span class="sxs-lookup"><span data-stu-id="f6bf5-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="f6bf5-109">เลือกมุม**มองตัวเลือก** \> **มุมมองในแฟ้ม Explorer**</span><span class="sxs-lookup"><span data-stu-id="f6bf5-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="f6bf5-110">ดูใน File Explorer เข้ากันไม่ได้กับ Microsoft Edge, Google โครเมียม, Firefox และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="f6bf5-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="f6bf5-111">**ดูใน File explorer**พร้อมใช้งานเฉพาะใน Internet Explorer เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="f6bf5-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="f6bf5-112">ตรวจสอบให้แน่ใจว่าบริการ WebClient กำลังทำงานอยู่</span><span class="sxs-lookup"><span data-stu-id="f6bf5-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="f6bf5-113">ในกล่องค้นหาของ Windows พิมพ์รันให้เลือกโปรแกรมประยุกต์การเรียกใช้เดสก์ท็อปพิมพ์บริการ. msc และจากนั้นกด Enter</span><span class="sxs-lookup"><span data-stu-id="f6bf5-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="f6bf5-114">เลื่อนลงไปที่บริการ WebClient และตรวจสอบให้แน่ใจว่าคอลัมน์**สถานะ**แสดง "กำลังทำงาน"</span><span class="sxs-lookup"><span data-stu-id="f6bf5-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="f6bf5-115">ถ้าไม่มีให้คลิกสองครั้งที่บริการคลิ**กเริ่ม**และจากนั้นคลิ**กตกลง**</span><span class="sxs-lookup"><span data-stu-id="f6bf5-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="f6bf5-116">(คุณอาจจำเป็นต้องเปิดใช้งานบริการด้วยการเลือก**ด้วยตนเอง**หรือ**อัตโนมัติ**ในกล่อง**ชนิดการเริ่มต้นระบบ**)</span><span class="sxs-lookup"><span data-stu-id="f6bf5-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="f6bf5-117">การเปิดไลบรารีใน File Explorer จะมีประโยชน์ถ้าคุณต้องการคัดลอกหรือย้ายไฟล์และโฟลเดอร์หลายครั้งแต่ถ้าคุณต้องการทำงานในไลบรารีเป็นประจำเราขอแนะนำให้ซิงค์ข้อมูลนั้น</span><span class="sxs-lookup"><span data-stu-id="f6bf5-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="f6bf5-118">หากต้องการแก้ไขปัญหาในการเปิด File Explorer โปรดดูที่[เปิดใน explorer](https://go.microsoft.com/fwlink/?linkid=871665)</span><span class="sxs-lookup"><span data-stu-id="f6bf5-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="f6bf5-119">สำหรับข้อมูลเกี่ยวกับการตั้งค่าการซิงค์โปรดดู[ที่การซิงค์แฟ้ม SharePoint กับไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://go.microsoft.com/fwlink/?linkid=871666)</span><span class="sxs-lookup"><span data-stu-id="f6bf5-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="f6bf5-120">โปรดดูบทความ[วิธีการใช้คำสั่ง "เปิดด้วย Explorer" เพื่อแก้ไขปัญหาใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="f6bf5-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

