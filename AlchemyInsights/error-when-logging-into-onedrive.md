---
title: 0x8004de40เปิด OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813671"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="eb701-102">0x8004de40เปิด OneDrive</span><span class="sxs-lookup"><span data-stu-id="eb701-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="eb701-103">ถ้าคุณได้รับข้อผิดพลาดเกี่ยวกับ **0x8004de40** เมื่อลงชื่อเข้าใช้ OneDrive ให้เริ่มระบบคอมพิวเตอร์ใหม่ขณะที่เชื่อมต่อกับโดเมนที่โรงเรียนหรือที่โรงเรียนของคุณ</span><span class="sxs-lookup"><span data-stu-id="eb701-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="eb701-104">ถ้าคุณได้รับข้อผิดพลาดนี้หลังจากเริ่มต้นระบบใหม่ ให้ลองวิธีนี้ขณะที่เชื่อมต่อกับโดเมนที่โรงเรียนหรือที่โรงเรียนของคุณ:</span><span class="sxs-lookup"><span data-stu-id="eb701-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="eb701-105">คลิก เริ่ม แล้วพิมพ์ **cmd** **หรือพร้อมท์**  ของสั่งในกล่องค้นหา คลิกขวาที่แอปพร้อมท์สั่ง  **แล้วเลือก เรียกใช้ในฐานะ** ผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="eb701-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="eb701-106">ถ้าคุณได้รับพร้อมท์ให้ใส่รหัสผ่านผู้ดูแลระบบหรือการยืนยัน ให้พิมพ์รหัสผ่าน หรือ **คลิก** อนุญาต</span><span class="sxs-lookup"><span data-stu-id="eb701-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="eb701-107">ในหน้าต่าง พร้อมท์สั่ง ให้พิมพ์ **dsregcmd /leave**  แล้วรอให้สั่งเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="eb701-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="eb701-108">จากนั้นพิมพ์ **dsregcmd /join** และรอให้สั่งเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="eb701-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="eb701-109">เริ่มระบบคอมพิวเตอร์ของคุณใหม่</span><span class="sxs-lookup"><span data-stu-id="eb701-109">Reboot your computer.</span></span>
