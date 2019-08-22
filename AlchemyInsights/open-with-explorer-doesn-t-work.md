---
title: เปิด ด้วย Explorer ไม่ทำงาน
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538507"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="4b89f-102">เปิด ด้วย Explorer ไม่ได้ทำงาน</span><span class="sxs-lookup"><span data-stu-id="4b89f-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="4b89f-103">ถ้า**เปิด ด้วย Explorer**หรือ**มุมมองใน Explorer แฟ้ม**ทำงานไม่ ตรวจสอบว่า บริการ WebClient ถูกตั้งค่าให้**เรียกใช้**โดยทำตามขั้นตอนด้านล่างนี้</span><span class="sxs-lookup"><span data-stu-id="4b89f-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="4b89f-104">ตัวอย่างเช่น ดังกล่าวอาจใช้เวลานานเมื่อต้องการเปิดไลบรารี SharePoint หรือ OneDrive เมื่อไม่ได้ทำงานการบริการ</span><span class="sxs-lookup"><span data-stu-id="4b89f-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="4b89f-105">ในกล่องค้นหาของ Windows ชนิดทำงาน เลือกเรียกใช้แอพลิเคชันเดสก์ท็อป ชนิด services.msc และจากนั้นเลือก**Enter**</span><span class="sxs-lookup"><span data-stu-id="4b89f-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="4b89f-106">เลื่อนลงไปยังบริการ WebClient และตรวจสอบคอลัมน์**สถานะ**</span><span class="sxs-lookup"><span data-stu-id="4b89f-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="4b89f-107">ถ้าสถานะของบริการ WebClient ไม่**ทำงาน**คลิกสองครั้งที่บริการ คลิก**เริ่ม**และจากนั้น คลิก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="4b89f-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="4b89f-108">เปิดใช้งานการบริการ ถ้าจำเป็น โดยเลือกอย่างใดอย่างหนึ่ง**ด้วยตนเอง**หรือ**โดยอัตโนมัติ**ในกล่อง**ชนิดการเริ่มต้น**</span><span class="sxs-lookup"><span data-stu-id="4b89f-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="4b89f-109">เมื่อต้องการแก้ไขปัญหาที่เปิดในแฟ้ม Explorer ดู[เปิดใน Explorer](https://go.microsoft.com/fwlink/?linkid=871665)</span><span class="sxs-lookup"><span data-stu-id="4b89f-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="4b89f-110">สำรวจข้อมูลให้ตรงกันเป็นทางเลือกดีกว่า: [SharePoint ซิงค์แฟ้มกับไคลเอนต์ซิงค์ OneDrive ใหม่](https://go.microsoft.com/fwlink/?linkid=871666)</span><span class="sxs-lookup"><span data-stu-id="4b89f-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

