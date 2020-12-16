---
title: การกำหนดรูปแบบโฮสต์ของเซสชันสำหรับเดสก์ท็อปเสมือนของ Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003902"
- "6957"
ms.openlocfilehash: 23bf130aad5bafa6756f0adfc2e58a130c2f6c4e
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692203"
---
# <a name="customize-a-session-host-image-for-windows-virtual-desktop"></a><span data-ttu-id="fa90d-102">การกำหนดรูปแบบโฮสต์ของเซสชันสำหรับเดสก์ท็อปเสมือนของ Windows</span><span class="sxs-lookup"><span data-stu-id="fa90d-102">Customize a session host image for Windows Virtual Desktop</span></span>

<span data-ttu-id="fa90d-103">มีสองวิธีในการจัดเตรียมเครื่องเสมือน (VM) โดยใช้รูปแบบเสมือนของฮาร์ดดิสก์เสมือนสำหรับเดสก์ท็อปเสมือนของ Windows:</span><span class="sxs-lookup"><span data-stu-id="fa90d-103">There are two ways to prepare a virtual machine (VM) by using a master Virtual Hard Disk image for Windows Virtual Desktop:</span></span>

1. <span data-ttu-id="fa90d-104">[สร้าง VM จากรูปที่ได้รับการจัดการใน Azure](https://go.microsoft.com/fwlink/?linkid=2127906)แล้วข้ามไปยังการ[จัดเตรียมและการติดตั้งซอฟต์แวร์](https://go.microsoft.com/fwlink/?linkid=2128064)</span><span class="sxs-lookup"><span data-stu-id="fa90d-104">[Create a VM from a managed image in Azure](https://go.microsoft.com/fwlink/?linkid=2127906), and then skip ahead to the [preparation and installation of software](https://go.microsoft.com/fwlink/?linkid=2128064).</span></span>
1. <span data-ttu-id="fa90d-105">[สร้างรูปภายในเครื่อง](https://go.microsoft.com/fwlink/?linkid=2128065) โดยการดาวน์โหลดรูปภาพการ [เตรียมใช้งาน Hyper V VM](https://go.microsoft.com/fwlink/?linkid=2127907)แล้วกำหนดค่าให้เหมาะสมกับความต้องการของคุณ</span><span class="sxs-lookup"><span data-stu-id="fa90d-105">[Create the image locally](https://go.microsoft.com/fwlink/?linkid=2128065) by downloading the image, [provisioning a Hyper-V VM](https://go.microsoft.com/fwlink/?linkid=2127907), and then customizing it to suit your needs.</span></span>

<span data-ttu-id="fa90d-106">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดู[ที่การเตรียมและกำหนดรูปแบบ VHD ต้นแบบ](https://go.microsoft.com/fwlink/?linkid=2127838)</span><span class="sxs-lookup"><span data-stu-id="fa90d-106">To learn more, see [Prepare and customize a master VHD image](https://go.microsoft.com/fwlink/?linkid=2127838).</span></span>