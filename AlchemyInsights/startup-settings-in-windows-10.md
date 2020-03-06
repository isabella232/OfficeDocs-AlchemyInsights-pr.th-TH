---
title: การตั้งค่าเริ่มต้นระบบใน Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409226"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="9bd64-102">การตั้งค่าเริ่มต้นระบบใน Windows 10</span><span class="sxs-lookup"><span data-stu-id="9bd64-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="9bd64-103">**เปลี่ยนแอปที่ทำงานโดยอัตโนมัติเมื่อเริ่มต้น**</span><span class="sxs-lookup"><span data-stu-id="9bd64-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="9bd64-104">ไปที่[การตั้งค่า > แอ > เริ่มต้นระบบ](ms-settings:startupapps?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="9bd64-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="9bd64-105">ตรวจสอบให้แน่ใจว่าแอปที่คุณต้องการเรียกใช้เมื่อเริ่ม**ต้นเปิดอยู่**</span><span class="sxs-lookup"><span data-stu-id="9bd64-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="9bd64-106">**เพิ่มแอปเพื่อทำงานโดยอัตโนมัติเมื่อเริ่มต้นระบบ**</span><span class="sxs-lookup"><span data-stu-id="9bd64-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="9bd64-107">คลิกหรือแตะ**เริ่มต้น**และค้นหาแอปที่คุณต้องการเรียกใช้เมื่อเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="9bd64-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="9bd64-108">คลิกขวาที่แอปคลิก**เพิ่มเติม**แล้วคลิก**เปิดตำแหน่งที่ตั้งแฟ้ม**</span><span class="sxs-lookup"><span data-stu-id="9bd64-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="9bd64-109">ซึ่งจะเปิดตำแหน่งที่ตั้งที่มีการบันทึกทางลัดไปยังแอป</span><span class="sxs-lookup"><span data-stu-id="9bd64-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="9bd64-110">ถ้าไม่มีตัวเลือกสำหรับตำแหน่งแฟ้มที่เปิดอยู่หมายความว่าแอพจะไม่สามารถเรียกใช้เมื่อเริ่มต้นระบบได้</span><span class="sxs-lookup"><span data-stu-id="9bd64-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="9bd64-111">ด้วยตำแหน่งที่ตั้งแฟ้มเปิดกด**โลโก้ Windows คีย์ + R**ชนิด**เชลล์: เริ่มต้น**แล้วคลิ**กตกลง**.</span><span class="sxs-lookup"><span data-stu-id="9bd64-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="9bd64-112">ซึ่งจะเปิดโฟลเดอร์เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="9bd64-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="9bd64-113">คัดลอกและวางทางลัดไปยังโปรแกรมประยุกต์จากตำแหน่งที่ตั้งแฟ้มไปยังโฟลเดอร์เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="9bd64-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="9bd64-114">**ตัวเลือกการเริ่มต้นขั้นสูง (รวมถึงเซฟโหมดการตั้งค่า UEFI และการเริ่มระบบจากอุปกรณ์อื่น)**</span><span class="sxs-lookup"><span data-stu-id="9bd64-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="9bd64-115">บันทึกงานของคุณและปิดเอกสารใดๆที่เปิดอยู่เนื่องจากขั้นตอนเหล่านี้จะรีสตาร์ทเครื่องคอมพิวเตอร์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="9bd64-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="9bd64-116">ไปที่การ[ตั้งค่า > การปรับปรุง & การรักษาความปลอดภัย > การกู้คืน](ms-settings:recovery?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="9bd64-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="9bd64-117">ภายใต้**เริ่มต้นขั้นสูง**คลิก**เริ่มระบบใหม่เดี๋ยวนี้**.</span><span class="sxs-lookup"><span data-stu-id="9bd64-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="9bd64-118">หลังจากที่พีซีของคุณเริ่มระบบใหม่เพื่อเลือกหน้าจอตัวเลือก:</span><span class="sxs-lookup"><span data-stu-id="9bd64-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="9bd64-119">เมื่อต้องการเริ่มระบบจากอุปกรณ์เช่นไดรฟ์ USB ให้คลิก**ใช้อุปกรณ์**</span><span class="sxs-lookup"><span data-stu-id="9bd64-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="9bd64-120">เมื่อต้องการป้อนการตั้งค่า UEFI (บางครั้งเรียกว่าการตั้งค่า BIOS) ให้คลิก**แก้ไขปัญหา > ตัวเลือกขั้นสูง > การตั้งค่าเฟิร์มแวร์ UEFI**</span><span class="sxs-lookup"><span data-stu-id="9bd64-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="9bd64-121">เมื่อต้องการเข้าสู่เซฟโหมดหรือเปลี่ยนการตั้งค่าเริ่มต้นขั้นสูงให้คลิก**แก้ไขปัญหา > ตัวเลือกขั้นสูง > การตั้งค่าเริ่มต้น**จากนั้นคลิก**เริ่มระบบใหม่**</span><span class="sxs-lookup"><span data-stu-id="9bd64-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="9bd64-122">คุณอาจถูกขอให้ป้อน[คีย์การกู้คืน BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)ของคุณ</span><span class="sxs-lookup"><span data-stu-id="9bd64-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="9bd64-123">หลังจากที่พีซีของคุณเริ่มระบบใหม่อีกครั้งให้คลิกการตั้งค่าเริ่มต้นที่คุณต้องการใช้</span><span class="sxs-lookup"><span data-stu-id="9bd64-123">After your PC restarts again, click the startup setting you want to use.</span></span>