---
title: การตั้งค่าการเริ่มต้นใน Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828171"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="a6471-102">การตั้งค่าการเริ่มต้นใน Windows 10</span><span class="sxs-lookup"><span data-stu-id="a6471-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="a6471-103">**เปลี่ยนแอปที่จะเล่นโดยอัตโนมัติเมื่อเริ่มต้นระบบ**</span><span class="sxs-lookup"><span data-stu-id="a6471-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="a6471-104">ไปที่[การตั้งค่า >แอป >เริ่มต้นระบบ](ms-settings:startupapps?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="a6471-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="a6471-105">ตรวจสอบให้แน่ใจว่าแอปใดๆ ที่คุณต้องการเรียกใช้เมื่อเริ่มต้นระบบ **เปิดอยู่**</span><span class="sxs-lookup"><span data-stu-id="a6471-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="a6471-106">**เพิ่มแอปให้เรียกใช้โดยอัตโนมัติเมื่อเริ่มต้นระบบ**</span><span class="sxs-lookup"><span data-stu-id="a6471-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="a6471-107">คลิกหรือ **แตะ** เริ่ม แล้วค้นหาแอปที่คุณต้องการเรียกใช้เมื่อเริ่มต้นระบบ</span><span class="sxs-lookup"><span data-stu-id="a6471-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="a6471-108">คลิกขวาที่แอป คลิก เพิ่มเติม แล้วคลิก **เปิด** ที่ตั้ง **ไฟล์**</span><span class="sxs-lookup"><span data-stu-id="a6471-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="a6471-109">ซึ่งจะเปิดที่ตั้งที่ทางลัดไปยังแอปถูกบันทึกไว้</span><span class="sxs-lookup"><span data-stu-id="a6471-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="a6471-110">ถ้าไม่มีตัวเลือกให้ เปิดที่ตั้งไฟล์ แสดงว่าแอปไม่สามารถเรียกใช้เมื่อเริ่มต้นระบบ</span><span class="sxs-lookup"><span data-stu-id="a6471-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="a6471-111">เมื่อเปิดที่ตั้งไฟล์แล้ว ให้ **กดแป้นโลโก้ Windows + R** พิมพ์ **shell:startup\*\*\*\*แล้วคลิก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="a6471-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="a6471-112">ซึ่งจะเปิดโฟลเดอร์เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="a6471-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="a6471-113">คัดลอกและวางทางลัดไปยังแอปจากที่ตั้งไฟล์ไปยังโฟลเดอร์เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="a6471-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="a6471-114">**ตัวเลือกการเริ่มต้นขั้นสูง (รวมถึงเซฟโหมด การตั้งค่า UEFI และการเริ่มต้นระบบจากอุปกรณ์อื่น)**</span><span class="sxs-lookup"><span data-stu-id="a6471-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="a6471-115">บันทึกงานของคุณและปิดเอกสารที่เปิดอยู่ เนื่องจากขั้นตอนเหล่านี้จะรีสตาร์ตพีซีของคุณ</span><span class="sxs-lookup"><span data-stu-id="a6471-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="a6471-116">ไปที่[การตั้งค่า >การอัปเดต&การรักษา>การกู้คืน](ms-settings:recovery?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="a6471-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="a6471-117">ภายใต้ **การเริ่มต้นขั้นสูง** ให้คลิก **รีสตาร์ต** เดี๋ยวนี้</span><span class="sxs-lookup"><span data-stu-id="a6471-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="a6471-118">หลังจากพีซีของคุณเริ่มระบบใหม่ไปยังหน้าจอ เลือกตัวเลือก:</span><span class="sxs-lookup"><span data-stu-id="a6471-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="a6471-119">เมื่อต้องการเริ่มระบบจากอุปกรณ์เช่นไดรฟ์ USB ให้คลิก **ใช้** อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="a6471-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="a6471-120">เมื่อต้องการใส่การตั้งค่า UEFI (บางครั้งเรียกว่าการตั้งค่า UEFI) ให้คลิก **>ตัวเลือกขั้นสูง >การตั้งค่าเฟิร์มแวร์ UEFI**</span><span class="sxs-lookup"><span data-stu-id="a6471-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="a6471-121">เมื่อต้องการใส่เซฟโหมดหรือเปลี่ยนการตั้งค่าเริ่มต้นขั้นสูง ให้คลิก **>การตั้งค่าขั้นสูง >การตั้งค่า** เริ่มต้น แล้วคลิก **รีสตาร์** ต</span><span class="sxs-lookup"><span data-stu-id="a6471-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="a6471-122">คุณอาจถูกขอให้ใส่คีย์การกู้คืน [BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)ของคุณ</span><span class="sxs-lookup"><span data-stu-id="a6471-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="a6471-123">หลังจากพีซีของคุณเริ่มระบบใหม่อีกครั้ง ให้คลิกการตั้งค่าเริ่มต้นระบบที่คุณต้องการใช้</span><span class="sxs-lookup"><span data-stu-id="a6471-123">After your PC restarts again, click the startup setting you want to use.</span></span>