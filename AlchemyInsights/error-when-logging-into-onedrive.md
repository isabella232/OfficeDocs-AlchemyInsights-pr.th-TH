---
title: ข้อผิดพลาด0x8004de40 เมื่อเปิดใช้งาน OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823120"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="b32d3-102">ข้อผิดพลาด0x8004de40 เมื่อเปิดใช้งาน OneDrive</span><span class="sxs-lookup"><span data-stu-id="b32d3-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="b32d3-103">ถ้าคุณได้รับข้อผิดพลาด **0x8004de40** เมื่อเข้าสู่ระบบ OneDrive ให้รีบูตเครื่องคอมพิวเตอร์ในขณะที่เชื่อมต่อกับโดเมนของที่ทำงานหรือที่โรงเรียนของคุณ</span><span class="sxs-lookup"><span data-stu-id="b32d3-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="b32d3-104">ถ้าคุณได้รับข้อผิดพลาดนี้หลังจากรีบูตให้ลองใช้วิธีนี้ในขณะที่เชื่อมต่อกับโดเมนของที่ทำงานหรือโรงเรียนของคุณ:</span><span class="sxs-lookup"><span data-stu-id="b32d3-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="b32d3-105">คลิกเริ่มแล้วพิมพ์ **cmd** หรือ **พร้อมท์คำสั่ง** ในกล่องค้นหาให้คลิกขวาบนแอปพร้อมท์คำสั่งแล้วเลือก **เรียกใช้ในฐานะผู้ดูแลระบบ**</span><span class="sxs-lookup"><span data-stu-id="b32d3-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="b32d3-106">ถ้าคุณได้รับพร้อมท์สำหรับรหัสผ่านผู้ดูแลระบบหรือการยืนยันให้พิมพ์รหัสผ่านหรือคลิก **อนุญาต**</span><span class="sxs-lookup"><span data-stu-id="b32d3-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="b32d3-107">ในหน้าต่างพร้อมท์คำสั่งให้พิมพ์ **dsregcmd/leave**  และรอให้คำสั่งเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="b32d3-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="b32d3-108">จากนั้นพิมพ์ **dsregcmd/join** และรอให้คำสั่งเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="b32d3-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="b32d3-109">เริ่มต้นระบบคอมพิวเตอร์ของคุณใหม่</span><span class="sxs-lookup"><span data-stu-id="b32d3-109">Reboot your computer.</span></span>
