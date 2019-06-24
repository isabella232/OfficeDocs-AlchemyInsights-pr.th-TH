---
title: แก้ไขข้อผิดพลาด 0x8004de40 ใน OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133995"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="01a82-102">แก้ไขข้อผิดพลาด 0x8004de40 ใน OneDrive</span><span class="sxs-lookup"><span data-stu-id="01a82-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="01a82-103">ถ้าคุณได้รับข้อผิดพลาด 0x8004de40 OneDrive:</span><span class="sxs-lookup"><span data-stu-id="01a82-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="01a82-104">รีบูตเครื่องคอมพิวเตอร์ได้รับผลกระทบในขณะที่เชื่อมต่อกับโดเมนของไดเรกทอรี Acitve ของคุณ</span><span class="sxs-lookup"><span data-stu-id="01a82-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="01a82-105">ถ้ามีการเริ่มระบบไม่สามารถแก้ไขปัญหา unjoin และข้อมูลอุปกรณ์ของคุณจากโฆษณา Azure</span><span class="sxs-lookup"><span data-stu-id="01a82-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="01a82-106">**หมายเหตุ**: คุณควรบนเครือข่ายขององค์กรของคุณในขณะที่กำลังดำเนินการขั้นตอนเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="01a82-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="01a82-107">ไม่ต้องทำขั้นตอนเหล่านี้เมื่อคุณไม่สามารถเชื่อมต่อกับโครงสร้างพื้นฐานขององค์กรของคุณ (ตัวอย่างเช่น ระหว่างการเดินทาง)</span><span class="sxs-lookup"><span data-stu-id="01a82-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="01a82-108">เปิดพร้อมท์คำสั่ง</span><span class="sxs-lookup"><span data-stu-id="01a82-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="01a82-109">เมื่อต้องการเปิดพร้อมท์คำสั่ง คลิ ก -**เริ่ม**คลิกขวาที่**หน้าจอพร้อมรับคำสั่ง**และ แล้ว คลิก**เรียกใช้ในฐานะผู้ดูแล**</span><span class="sxs-lookup"><span data-stu-id="01a82-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="01a82-110">พิมพ์*dsregcmd /leave*และกด**Enter**</span><span class="sxs-lookup"><span data-stu-id="01a82-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="01a82-111">เมื่อเสร็จสิ้น พิมพ์*dsregcmd /join*และกด**Enter**</span><span class="sxs-lookup"><span data-stu-id="01a82-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="01a82-112">เมื่อเสร็จสิ้น ปิดพรอมต์คำสั่ง</span><span class="sxs-lookup"><span data-stu-id="01a82-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="01a82-113">รีบูตเครื่องคอมพิวเตอร์ และเข้าสู่ระบบไปยัง OneDrive</span><span class="sxs-lookup"><span data-stu-id="01a82-113">Reboot the computer, and log into OneDrive.</span></span>