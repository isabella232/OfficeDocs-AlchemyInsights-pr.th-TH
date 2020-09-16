---
title: แก้ไขข้อผิดพลาด0x8004de40 ใน OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745149"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="4f75e-102">แก้ไขข้อผิดพลาด0x8004de40 ใน OneDrive</span><span class="sxs-lookup"><span data-stu-id="4f75e-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="4f75e-103">ถ้าคุณได้รับข้อผิดพลาด0x8004de40 กับ OneDrive:</span><span class="sxs-lookup"><span data-stu-id="4f75e-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="4f75e-104">รีบูตเครื่องคอมพิวเตอร์ที่ได้รับผลกระทบในขณะที่เชื่อมต่อกับโดเมนไดเรกทอรี Acitve ของคุณ</span><span class="sxs-lookup"><span data-stu-id="4f75e-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="4f75e-105">ถ้าการรีบูทไม่สามารถแก้ไขปัญหาได้ให้เลิกและเข้าร่วมอุปกรณ์ของคุณจาก Azure AD</span><span class="sxs-lookup"><span data-stu-id="4f75e-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="4f75e-106">**หมายเหตุ**: คุณควรอยู่บนเครือข่ายขององค์กรของคุณในขณะที่ดำเนินการขั้นตอนเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="4f75e-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="4f75e-107">อย่าทำตามขั้นตอนเหล่านี้เมื่อคุณไม่สามารถเชื่อมต่อกับโครงสร้างพื้นฐานขององค์กรของคุณ (ตัวอย่างเช่นในขณะเดินทาง)</span><span class="sxs-lookup"><span data-stu-id="4f75e-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="4f75e-108">เปิดพร้อมท์คำสั่งยกระดับ</span><span class="sxs-lookup"><span data-stu-id="4f75e-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="4f75e-109">เมื่อต้องการเปิดพร้อมท์คำสั่งยกระดับให้คลิก-**เริ่ม**แล้วคลิกขวาที่**พร้อมท์คำสั่ง**แล้วคลิก**เรียกใช้ในฐานะผู้ดูแลระบบ**</span><span class="sxs-lookup"><span data-stu-id="4f75e-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="4f75e-110">พิมพ์*dsregcmd/leave*แล้วกด**Enter**</span><span class="sxs-lookup"><span data-stu-id="4f75e-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="4f75e-111">เมื่อทำเสร็จแล้วให้พิมพ์*dsregcmd/join*แล้วกด**Enter**</span><span class="sxs-lookup"><span data-stu-id="4f75e-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="4f75e-112">เมื่อทำเสร็จแล้วให้ปิดพร้อมท์คำสั่ง</span><span class="sxs-lookup"><span data-stu-id="4f75e-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="4f75e-113">รีบูตเครื่องคอมพิวเตอร์แล้วเข้าสู่ระบบ OneDrive</span><span class="sxs-lookup"><span data-stu-id="4f75e-113">Reboot the computer, and log into OneDrive.</span></span>