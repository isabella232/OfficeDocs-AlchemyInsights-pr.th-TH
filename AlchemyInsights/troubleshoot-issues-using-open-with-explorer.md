---
title: แก้ปัญหาโดยใช้เปิด ด้วย Explorer
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
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390626"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="da6d5-102">แก้ปัญหาเกี่ยวกับการเปิดด้วย Explorer</span><span class="sxs-lookup"><span data-stu-id="da6d5-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="da6d5-103">แก้ไขปัญหาทั่วไปเกี่ยวกับการเปิดไลบรารีเอกสารใน SharePoint หรือ OneDrive โดยใช้คำสั่ง**เปิด ด้วย Explorer** :</span><span class="sxs-lookup"><span data-stu-id="da6d5-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="da6d5-104">ใช้ Internet Explorer 10 หรือ Internet Explorer 11</span><span class="sxs-lookup"><span data-stu-id="da6d5-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="da6d5-105">**เปิด ด้วย Explorer**ไม่เข้ากันกับ Microsoft ขอบ Google โครเมียม Firefox และผู้อื่น</span><span class="sxs-lookup"><span data-stu-id="da6d5-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="da6d5-106">**เปิด ด้วย Explorer**ถูกปิดใช้งานในเบราว์เซอร์ทั้งหมดยกเว้น Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="da6d5-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="da6d5-107">**เปิด ด้วย Explorer**จะไม่พร้อมใช้งานในประสบการณ์ใช้งานแบบสมัยใหม่สำหรับไลบรารี SharePoint</span><span class="sxs-lookup"><span data-stu-id="da6d5-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="da6d5-108">ใช้**มุมมองใน Explorer แฟ้ม**แทน</span><span class="sxs-lookup"><span data-stu-id="da6d5-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="da6d5-109">เลือก**ตัวเลือกมุมมอง** \> **มุมมอง Explorer แฟ้ม**</span><span class="sxs-lookup"><span data-stu-id="da6d5-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="da6d5-110">มุมมองใน Explorer แฟ้มเข้ากันไม่ได้กับ ขอบของ Microsoft, Google โครเมียม Firefox และอื่น ๆ</span><span class="sxs-lookup"><span data-stu-id="da6d5-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="da6d5-111">**มุมมองใน Explorer แฟ้ม**ในพร้อมใช้งานเฉพาะใน Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="da6d5-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="da6d5-112">ตรวจสอบให้แน่ใจว่า กำลังเรียกใช้บริการ WebClient</span><span class="sxs-lookup"><span data-stu-id="da6d5-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="da6d5-113">ใน Windows กล่องค้นหา ชนิดทำงาน เลือกเรียกใช้เดสก์ท็อปแอพลิเคชัน พิมพ์ services.msc และจากนั้น กด Enter</span><span class="sxs-lookup"><span data-stu-id="da6d5-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="da6d5-114">เลื่อนลงไปยังบริการ WebClient และต้องแน่ใจว่า คอลัมน์**สถานะ**แสดง "รัน"</span><span class="sxs-lookup"><span data-stu-id="da6d5-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="da6d5-115">หากโปรแกรมไม่ คลิกสองครั้งที่บริการ คลิก**เริ่ม**และจากนั้น คลิก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="da6d5-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="da6d5-116">(คุณอาจจำเป็นต้องเปิดใช้งานการบริการก่อน โดยเลือกอย่างใดอย่างหนึ่ง**ด้วยตนเอง**หรือ**โดยอัตโนมัติ**ในกล่อง**ชนิดการเริ่มต้นระบบ**)</span><span class="sxs-lookup"><span data-stu-id="da6d5-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="da6d5-117">เปิดไลบรารีในแฟ้ม Explorer จะสะดวกถ้าคุณต้องการคัดลอก หรือย้ายแฟ้มและโฟลเดอร์หลายทันที แต่ ถ้าคุณต้องการทำงานเป็นประจำในไลบรารี เราขอแนะนำให้ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="da6d5-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="da6d5-118">เมื่อต้องการแก้ไขปัญหาที่เปิดในแฟ้ม Explorer ดู[เปิดใน Explorer](https://go.microsoft.com/fwlink/?linkid=871665)</span><span class="sxs-lookup"><span data-stu-id="da6d5-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="da6d5-119">สำหรับข้อมูลเกี่ยวกับการตั้งค่าการซิงค์ ดู[SharePoint ซิงค์แฟ้มกับไคลเอนต์ซิงค์ OneDrive ใหม่](https://go.microsoft.com/fwlink/?linkid=871666)</span><span class="sxs-lookup"><span data-stu-id="da6d5-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="da6d5-120">โปรดดูบทความ[วิธีใช้คำสั่ง "เปิดด้วย Explorer " การแก้ไขปัญหาใน SharePoint แบบออนไลน์](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="da6d5-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

