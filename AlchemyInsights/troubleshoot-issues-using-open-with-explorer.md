---
title: แก้ไขปัญหาการใช้ Open กับ Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759711"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="cc227-102">แก้ไขปัญหาเกี่ยวกับเปิดด้วย Explorer</span><span class="sxs-lookup"><span data-stu-id="cc227-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="cc227-103">แก้ไขปัญหาทั่วไปเกี่ยวกับการเปิดไลบรารีเอกสารใน SharePoint หรือ OneDrive**โดยใช้คําสั่ง**</span><span class="sxs-lookup"><span data-stu-id="cc227-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="cc227-104">ใช้ 10 Explorer อินเทอร์เน็ตหรือ 11 Explorer อินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="cc227-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="cc227-105">**เปิดด้วย Explorer**ไม่เข้ากันได้กับไมโครซอฟท์ขอบ, Google Chrome, Firefox และอื่น ๆ.</span><span class="sxs-lookup"><span data-stu-id="cc227-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="cc227-106">**เปิดด้วย Explorer**ถูกปิดใช้งานในเบราว์เซอร์ทั้งหมดยกเว้น Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="cc227-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="cc227-107">**เปิดด้วย Explorer**ไม่พร้อมใช้งานในประสบการณ์ใช้งานที่ทันสมัยสําหรับไลบรารี SharePoint</span><span class="sxs-lookup"><span data-stu-id="cc227-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="cc227-108">ใช้**มุมมองในแฟ้ม Explorer**แทน</span><span class="sxs-lookup"><span data-stu-id="cc227-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="cc227-109">เลือก**มุมมอง ตัวเลือก**\>**มุมมอง ใน File Explorer**</span><span class="sxs-lookup"><span data-stu-id="cc227-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="cc227-110">ดูในไฟล์ Explorer ไม่เข้ากันได้กับไมโครซอฟท์ขอบ, Google Chrome, Firefox และอื่น ๆ.</span><span class="sxs-lookup"><span data-stu-id="cc227-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="cc227-111">**ดูในแฟ้ม Explorer**ในพร้อมใช้งานใน Internet Explorer เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="cc227-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="cc227-112">ตรวจสอบให้แน่ใจว่าบริการ WebClient กําลังทํางานอยู่</span><span class="sxs-lookup"><span data-stu-id="cc227-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="cc227-113">ในกล่องค้นหาของ Windows ให้พิมพ์ เรียกใช้ เลือกเรียกใช้โปรแกรมประยุกต์บนเดสก์ท็อป</span><span class="sxs-lookup"><span data-stu-id="cc227-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="cc227-114">เลื่อนลงไปยังบริการ WebClient และตรวจสอบให้แน่ใจว่าคอลัมน์**สถานะ**แสดง "ทํางาน"</span><span class="sxs-lookup"><span data-stu-id="cc227-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="cc227-115">ถ้าบริการไม่แสดงให้คลิกสองครั้งที่บริการ แล้วคลิก**เริ่ม**แล้วคลิก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="cc227-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="cc227-116">(คุณอาจต้องเปิดใช้งานบริการโดยการเลือก**ด้วยตนเอง**หรือ**อัตโนมัติ**ในกล่อง**ชนิดการเริ่มต้น**)</span><span class="sxs-lookup"><span data-stu-id="cc227-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="cc227-117">การเปิดไลบรารีใน File Explorer มีประโยชน์หากคุณต้องการคัดลอกหรือย้ายหลายไฟล์และโฟลเดอร์หนึ่งครั้ง แต่ถ้าคุณต้องการทํางานอย่างสม่ําเสมอในไลบรารีเราขอแนะนําให้ซิงค์</span><span class="sxs-lookup"><span data-stu-id="cc227-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="cc227-118">เมื่อต้องการแก้ไขปัญหาการเปิดใน File Explorer ให้ดูที่[เปิดใน Explorer](https://go.microsoft.com/fwlink/?linkid=871665)</span><span class="sxs-lookup"><span data-stu-id="cc227-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="cc227-119">สําหรับข้อมูลเกี่ยวกับการตั้งค่าการซิงค์ ให้ดูที่[ซิงค์ไฟล์ SharePoint กับไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://go.microsoft.com/fwlink/?linkid=871666)</span><span class="sxs-lookup"><span data-stu-id="cc227-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="cc227-120">โปรดดูบทความ[วิธีการใช้คําสั่ง "เปิดด้วย Explorer" เพื่อแก้ไขปัญหาใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="cc227-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

