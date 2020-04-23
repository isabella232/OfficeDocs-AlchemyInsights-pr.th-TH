---
title: แก้ไขข้อผิดพลาด 0x8004de40 ใน OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716047"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="0cfb1-102">แก้ไขข้อผิดพลาด 0x8004de40 ใน OneDrive</span><span class="sxs-lookup"><span data-stu-id="0cfb1-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="0cfb1-103">ถ้าคุณได้รับข้อผิดพลาด 0x8004de40 ด้วย OneDrive:</span><span class="sxs-lookup"><span data-stu-id="0cfb1-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="0cfb1-104">รีบูตเครื่องคอมพิวเตอร์ที่ได้รับผลกระทบในขณะที่เชื่อมต่อกับโดเมนไดเรกทอรี Acitve ของคุณ</span><span class="sxs-lookup"><span data-stu-id="0cfb1-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="0cfb1-105">ถ้าการเริ่มระบบใหม่ไม่สามารถแก้ไขปัญหา ให้ยกเลิกเข้าร่วม และเข้าร่วมอุปกรณ์ของคุณจาก Azure AD อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="0cfb1-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="0cfb1-106">**หมายเหตุ**: คุณควรอยู่ในเครือข่ายองค์กรของคุณในขณะที่ทําตามขั้นตอนเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="0cfb1-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="0cfb1-107">อย่าทําตามขั้นตอนเหล่านี้เมื่อคุณไม่สามารถเชื่อมต่อกับโครงสร้างพื้นฐานขององค์กรได้ (เช่น ขณะเดินทาง)</span><span class="sxs-lookup"><span data-stu-id="0cfb1-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="0cfb1-108">เปิดพร้อมท์คําสั่ง</span><span class="sxs-lookup"><span data-stu-id="0cfb1-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="0cfb1-109">เมื่อต้องการเปิดพร้อมท์คําสั่ง ให้คลิก -**เริ่ม**คลิกขวาที่**พร้อมท์คําสั่ง**แล้วคลิก**เรียกใช้ในฐานะผู้ดูแลระบบ**</span><span class="sxs-lookup"><span data-stu-id="0cfb1-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="0cfb1-110">พิมพ์*dsregcmd /leave*และกด**Enter**</span><span class="sxs-lookup"><span data-stu-id="0cfb1-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="0cfb1-111">เมื่อเสร็จสมบูรณ์*dsregcmd /join\*\*\*Enter*\*</span><span class="sxs-lookup"><span data-stu-id="0cfb1-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="0cfb1-112">เมื่อเสร็จสิ้น ให้ปิดพรอมต์คําสั่ง</span><span class="sxs-lookup"><span data-stu-id="0cfb1-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="0cfb1-113">รีบูตเครื่องคอมพิวเตอร์ และเข้าสู่ระบบ OneDrive</span><span class="sxs-lookup"><span data-stu-id="0cfb1-113">Reboot the computer, and log into OneDrive.</span></span>