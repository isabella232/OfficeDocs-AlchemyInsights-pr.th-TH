---
title: เปิดด้วย Explorer ไม่ทํางาน
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713053"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="771e1-102">เปิดด้วยโปรแกรมสํารวจไม่ทํางาน</span><span class="sxs-lookup"><span data-stu-id="771e1-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="771e1-103">ถ้า**เปิดด้วย Explorer**หรือ**มุมมองในแฟ้ม Explorer**ไม่ทํางาน โปรดตรวจสอบให้แน่ใจว่า บริการ WebClient ถูกตั้งค่า**เป็น ทํางาน**โดยทําตามขั้นตอนด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="771e1-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="771e1-104">ตัวอย่างเช่น อาจใช้เวลานานในการเปิดไลบรารี SharePoint หรือ OneDrive เมื่อไม่ได้เรียกใช้บริการ</span><span class="sxs-lookup"><span data-stu-id="771e1-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="771e1-105">ในกล่องค้นหาของ Windows ให้พิมพ์ เรียกใช้ เลือกเรียกใช้แอปเดสก์ท็อป**Enter**</span><span class="sxs-lookup"><span data-stu-id="771e1-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="771e1-106">เลื่อนลงไปที่บริการ WebClient และตรวจสอบคอลัมน์**สถานะ**</span><span class="sxs-lookup"><span data-stu-id="771e1-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="771e1-107">ถ้าสถานะการบริการ WebClient ไม่ได้**ทํางาน**อยู่ ให้คลิกสองครั้งที่บริการ คลิก**เริ่ม**แล้วคลิก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="771e1-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="771e1-108">เปิดใช้งานบริการ ถ้าจําเป็น โดยการเลือก**ด้วยตนเอง**หรือ**อัตโนมัติ**ในกล่อง**ชนิดการเริ่มต้น**ระบบ</span><span class="sxs-lookup"><span data-stu-id="771e1-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="771e1-109">เมื่อต้องการแก้ไขปัญหาการเปิดใน File Explorer ให้ดูที่[เปิดใน Explorer](https://go.microsoft.com/fwlink/?linkid=871665)</span><span class="sxs-lookup"><span data-stu-id="771e1-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="771e1-110">สํารวจการซิงค์เป็นทางเลือกที่ดีกว่า:[ซิงค์ไฟล์ SharePoint กับไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://go.microsoft.com/fwlink/?linkid=871666)</span><span class="sxs-lookup"><span data-stu-id="771e1-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

