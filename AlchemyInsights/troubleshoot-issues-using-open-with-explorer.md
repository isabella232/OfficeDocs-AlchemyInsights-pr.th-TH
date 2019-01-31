---
title: แก้ปัญหาโดยใช้เปิด ด้วย Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: c95f07b9fb7251442577c014e4005dbe3f92ceb4
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661770"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="8c3af-102">แก้ปัญหาเกี่ยวกับการเปิดด้วย Explorer</span><span class="sxs-lookup"><span data-stu-id="8c3af-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="8c3af-103">แก้ไขปัญหาทั่วไปเกี่ยวกับการเปิดไลบรารีเอกสารใน SharePoint หรือ OneDrive โดยใช้คำสั่ง**เปิด ด้วย Explorer** :</span><span class="sxs-lookup"><span data-stu-id="8c3af-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="8c3af-p101">ใช้ Internet Explorer 10 หรือ Internet Explorer 11 **เปิด ด้วย Explorer**ไม่เข้ากันกับ Microsoft ขอบ Google โครเมียม Firefox และผู้อื่น **เปิด ด้วย Explorer**ถูกปิดใช้งานในเบราว์เซอร์ทั้งหมดยกเว้น Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="8c3af-p101">Use Internet Explorer 10 or Internet Explorer 11. **Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others. **Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="8c3af-p102">**เปิด ด้วย Explorer**จะไม่พร้อมใช้งานในประสบการณ์ใช้งานแบบสมัยใหม่สำหรับไลบรารี SharePoint ใช้**มุมมองใน Explorer แฟ้ม**แทน เลือก**ตัวเลือกมุมมอง** \> **มุมมอง Explorer แฟ้ม** มุมมองใน Explorer แฟ้มเข้ากันไม่ได้กับ ขอบของ Microsoft, Google โครเมียม Firefox และอื่น ๆ **มุมมองใน Explorer แฟ้ม**ในพร้อมใช้งานเฉพาะใน Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="8c3af-p102">**Open with Explorer** is not available in the modern experience for SharePoint libraries. Use **View in File Explorer** instead. Select **View options** \> **View in File Explorer**. View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others. **View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="8c3af-p103">ตรวจสอบให้แน่ใจว่า กำลังเรียกใช้บริการ WebClient ใน Windows กล่องค้นหา ชนิดทำงาน เลือกเรียกใช้เดสก์ท็อปแอพลิเคชัน พิมพ์ services.msc และจากนั้น กด Enter เลื่อนลงไปยังบริการ WebClient และต้องแน่ใจว่า คอลัมน์**สถานะ**แสดง "รัน" หากโปรแกรมไม่ คลิกสองครั้งที่บริการ คลิก**เริ่ม**และจากนั้น คลิก**ตกลง** (คุณอาจจำเป็นต้องเปิดใช้งานการบริการก่อน โดยเลือกอย่างใดอย่างหนึ่ง**ด้วยตนเอง**หรือ**โดยอัตโนมัติ**ในกล่อง**ชนิดการเริ่มต้นระบบ**)</span><span class="sxs-lookup"><span data-stu-id="8c3af-p103">Make sure the WebClient service is running. In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter. Scroll down to the WebClient service and make sure the **Status** column displays "Running." If it doesn't, double-click the service, click **Start**, and then click **OK**. (You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8c3af-p104">เปิดไลบรารีในแฟ้ม Explorer จะสะดวกถ้าคุณต้องการคัดลอก หรือย้ายแฟ้มและโฟลเดอร์หลายทันที แต่ ถ้าคุณต้องการทำงานเป็นประจำในไลบรารี เราขอแนะนำให้ตรงกัน เมื่อต้องการแก้ไขปัญหาที่เปิดในแฟ้ม Explorer ดู[เปิดใน Explorer](https://go.microsoft.com/fwlink/?linkid=871665) สำหรับข้อมูลเกี่ยวกับการตั้งค่าการซิงค์ ดู[SharePoint ซิงค์แฟ้มกับไคลเอนต์ซิงค์ OneDrive ใหม่](https://go.microsoft.com/fwlink/?linkid=871666)</span><span class="sxs-lookup"><span data-stu-id="8c3af-p104">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it. To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="8c3af-120">โปรดดูบทความ[วิธีใช้คำสั่ง "เปิดด้วย Explorer " การแก้ไขปัญหาใน SharePoint แบบออนไลน์](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="8c3af-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

