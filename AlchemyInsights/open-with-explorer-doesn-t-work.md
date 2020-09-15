---
title: เปิดด้วย Explorer ไม่ทำงาน
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694475"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="22705-102">เปิดด้วย Explorer ไม่ทำงาน</span><span class="sxs-lookup"><span data-stu-id="22705-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="22705-103">ถ้า **เปิดด้วย Explorer** หรือ **มุมมองใน File Explorer** ไม่ทำงานให้ตรวจสอบให้แน่ใจว่าบริการ WebClient ถูกตั้งค่าให้ **ทำงานโดยทำ** ตามขั้นตอนด้านล่างนี้</span><span class="sxs-lookup"><span data-stu-id="22705-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="22705-104">ตัวอย่างเช่นอาจใช้เวลานานในการเปิดไลบรารี SharePoint หรือ OneDrive เมื่อบริการไม่ได้ทำงานอยู่</span><span class="sxs-lookup"><span data-stu-id="22705-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="22705-105">ในกล่องค้นหาของ Windows ให้พิมพ์เรียกใช้เลือกแอปเรียกใช้เดสก์ท็อปพิมพ์ services. msc แล้วเลือก**Enter**</span><span class="sxs-lookup"><span data-stu-id="22705-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="22705-106">เลื่อนลงไปยังบริการ WebClient แล้วตรวจสอบคอลัมน์**สถานะ**</span><span class="sxs-lookup"><span data-stu-id="22705-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="22705-107">ถ้าสถานะบริการ WebClient ไม่ได้**ทำงาน**อยู่ให้ดับเบิลคลิกที่บริการดังกล่าวแล้วคลิก**เริ่ม**แล้วคลิก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="22705-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="22705-108">เปิดใช้งานบริการถ้าจำเป็นโดยเลือก**ด้วยตนเอง**หรือ**โดยอัตโนมัติ**ในกล่อง**ชนิดการเริ่มต้น**</span><span class="sxs-lookup"><span data-stu-id="22705-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="22705-109">เมื่อต้องการแก้ไขปัญหาการเปิดใน File Explorer ให้ดูที่[เปิดใน Explorer](https://go.microsoft.com/fwlink/?linkid=871665)</span><span class="sxs-lookup"><span data-stu-id="22705-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="22705-110">สำรวจการซิงค์เป็นทางเลือกที่ดียิ่งขึ้น:[ซิงค์ไฟล์ SharePoint กับไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://go.microsoft.com/fwlink/?linkid=871666)</span><span class="sxs-lookup"><span data-stu-id="22705-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

