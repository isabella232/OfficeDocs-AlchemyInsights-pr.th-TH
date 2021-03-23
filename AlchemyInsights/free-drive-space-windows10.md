---
title: เพิ่มเนื้อที่ว่างบนไดรฟ์ใน Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037951"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="cb5d4-102">เพิ่มเนื้อที่ว่างบนไดรฟ์ใน Windows 10</span><span class="sxs-lookup"><span data-stu-id="cb5d4-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="cb5d4-103">ต่อไปนี้มีสองตัวเลือกในการเพิ่มเนื้อที่ว่างบนไดรฟ์ใน Windows:</span><span class="sxs-lookup"><span data-stu-id="cb5d4-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="cb5d4-104">เพิ่มเนื้อที่ว่างบนไดรฟ์ใน Windows 10</span><span class="sxs-lookup"><span data-stu-id="cb5d4-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="cb5d4-105">เพิ่มเนื้อที่ว่างการอัปเดต Windows 10 ด้วยอุปกรณ์เก็บข้อมูลภายนอก</span><span class="sxs-lookup"><span data-stu-id="cb5d4-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="cb5d4-106">ถ้าคุณยังมีเนื้อที่ว่างบนดิสก์เหลือน้อยหลังจากใช้การล้างข้อมูลบนดิสก์ อาจเป็นไปได้ว่าโฟลเดอร์ Temp ของคุณถูกเติมด้วยไฟล์แอปพลิเคชัน (.appx) ที่ใช้โดย Microsoft Store อย่างรวดเร็ว</span><span class="sxs-lookup"><span data-stu-id="cb5d4-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="cb5d4-107">เมื่อต้องการแก้ไขปัญหานี้ ให้รีเซ็ต Store ล้างแคช Store แล้วเรียกใช้ตัวแก้ไขปัญหา Windows Update</span><span class="sxs-lookup"><span data-stu-id="cb5d4-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="cb5d4-108">ตรวจสอบให้แน่ใจว่า Microsoft Store ปิดอยู่ก่อนที่คุณจะดําเนินการตามขั้นตอนเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="cb5d4-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="cb5d4-109">**ขั้นตอนที่ 1: รีเซ็ต Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="cb5d4-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="cb5d4-110">**หมายเหตุ** วิธีนี้จะลบข้อมูลแอปบนอุปกรณ์อย่างถาวร รวมถึงการตั้งค่าและรายละเอียดการลงชื่อเข้าใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="cb5d4-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="cb5d4-111">เลือก **เริ่ม**  >    >  **แอป**  >  **การตั้งค่าและ&คุณลักษณะบางอย่าง**</span><span class="sxs-lookup"><span data-stu-id="cb5d4-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="cb5d4-112">ในรายการแอป ให้ค้นหาและเลือก Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="cb5d4-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="cb5d4-113">เลือกตัวเลือก **ขั้นสูง**</span><span class="sxs-lookup"><span data-stu-id="cb5d4-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="cb5d4-114">เลื่อนลงและเลือก **รีเซ็ต** จากนั้น **ยืนยันการ** รีเซ็ต</span><span class="sxs-lookup"><span data-stu-id="cb5d4-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="cb5d4-115">**ขั้นตอนที่ 2: ล้างแคช Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="cb5d4-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="cb5d4-116">กดแป้นโลโก้ Windows + R เพื่อเปิดกล่องโต้ตอบ เรียกใช้</span><span class="sxs-lookup"><span data-stu-id="cb5d4-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="cb5d4-117">พิมพ์ wsreset.exe **แล้วเลือก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="cb5d4-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="cb5d4-118">หน้าต่าง พร้อมท์สั่ง เปล่า จะเปิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="cb5d4-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="cb5d4-119">หลังจากผ่านไปประมาณ 10 วินาที หน้าต่างจะปิดและ Store จะเปิดขึ้นโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="cb5d4-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="cb5d4-120">**ขั้นตอนที่ 3: รีเซ็ต Windows Update**</span><span class="sxs-lookup"><span data-stu-id="cb5d4-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="cb5d4-121">เลือก **เริ่ม**  >  **การอัปเดต**  >  **การตั้งค่า &แก้ไขปัญหา**  >  **ด้านความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="cb5d4-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="cb5d4-122">เลื่อนลงและเลือก **Windows Update** จากรายการ และเลือก **เรียกใช้ตัว** แก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="cb5d4-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="cb5d4-123">เริ่มระบบคอมพิวเตอร์ของคุณใหม่ แล้วตรวจสอบว่าคุณยังคงพบปัญหาหรือไม่</span><span class="sxs-lookup"><span data-stu-id="cb5d4-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

