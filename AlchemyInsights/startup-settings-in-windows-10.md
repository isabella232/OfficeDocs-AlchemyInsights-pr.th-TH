---
title: การตั้งค่าการเริ่มต้นใน Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751154"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="251d9-102">การตั้งค่าการเริ่มต้นใน Windows 10</span><span class="sxs-lookup"><span data-stu-id="251d9-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="251d9-103">**เปลี่ยนแอปที่ทำงานโดยอัตโนมัติเมื่อเริ่มต้น**</span><span class="sxs-lookup"><span data-stu-id="251d9-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="251d9-104">ไปที่ [การตั้งค่า > แอป > เริ่มต้น](ms-settings:startupapps?activationSource=GetHelp)ใช้งาน</span><span class="sxs-lookup"><span data-stu-id="251d9-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="251d9-105">ตรวจสอบให้แน่ใจว่าคุณต้องการเรียกใช้แอปที่คุณต้องการเรียกใช้เมื่อเริ่ม**ต้นเปิดใช้งานแล้ว**</span><span class="sxs-lookup"><span data-stu-id="251d9-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="251d9-106">**เพิ่มแอปเพื่อทำงานโดยอัตโนมัติเมื่อเริ่มต้น**</span><span class="sxs-lookup"><span data-stu-id="251d9-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="251d9-107">คลิกหรือแตะ **เริ่ม** และค้นหาแอปที่คุณต้องการเรียกใช้เมื่อเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="251d9-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="251d9-108">คลิกขวาที่แอปแล้วคลิก**เพิ่มเติม**แล้วคลิก**เปิดตำแหน่งที่ตั้งไฟล์**</span><span class="sxs-lookup"><span data-stu-id="251d9-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="251d9-109">ซึ่งจะเป็นการเปิดตำแหน่งที่ตั้งที่มีการบันทึกทางลัดไปยังแอป</span><span class="sxs-lookup"><span data-stu-id="251d9-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="251d9-110">ถ้าไม่มีตัวเลือกสำหรับการเปิดตำแหน่งที่ตั้งไฟล์แสดงว่าแอปไม่สามารถเรียกใช้ได้เมื่อเริ่มต้นใช้งาน</span><span class="sxs-lookup"><span data-stu-id="251d9-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="251d9-111">เมื่อเปิดตำแหน่งที่ตั้งไฟล์แล้วให้กด**แป้นโลโก้ Windows + R**แล้วพิมพ์**shell: เริ่มต้น**แล้วคลิก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="251d9-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="251d9-112">ซึ่งจะเป็นการเปิดโฟลเดอร์เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="251d9-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="251d9-113">คัดลอกและวางทางลัดไปยังแอปจากตำแหน่งที่ตั้งไฟล์ไปยังโฟลเดอร์เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="251d9-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="251d9-114">**ตัวเลือกการเริ่มต้นขั้นสูง (รวมถึงเซฟโหมดการตั้งค่า UEFI และการเริ่มระบบจากอุปกรณ์อื่น)**</span><span class="sxs-lookup"><span data-stu-id="251d9-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="251d9-115">บันทึกงานของคุณและปิดเอกสารใดๆที่เปิดอยู่เนื่องจากขั้นตอนเหล่านี้จะเริ่มต้นระบบพีซีของคุณใหม่</span><span class="sxs-lookup"><span data-stu-id="251d9-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="251d9-116">ไปที่การ[ตั้งค่า > การอัปเด & การรักษาความปลอดภัย > การกู้คืน](ms-settings:recovery?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="251d9-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="251d9-117">ภายใต้**เริ่มต้นขั้นสูง**ให้คลิก**เริ่มใหม่เดี๋ยวนี้**</span><span class="sxs-lookup"><span data-stu-id="251d9-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="251d9-118">หลังจากรีสตาร์ตพีซีของคุณไปยังหน้าจอเลือกตัวเลือก:</span><span class="sxs-lookup"><span data-stu-id="251d9-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="251d9-119">เมื่อต้องการเริ่มต้นระบบจากอุปกรณ์เช่นไดรฟ์ USB ให้คลิก**ใช้อุปกรณ์**</span><span class="sxs-lookup"><span data-stu-id="251d9-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="251d9-120">เมื่อต้องการเข้าสู่การตั้งค่า UEFI (บางครั้งเรียกว่าการตั้งค่า BIOS) ให้คลิก**แก้ไขปัญหา > ตัวเลือกขั้นสูง > การตั้งค่าเฟิร์มแวร์ UEFI**</span><span class="sxs-lookup"><span data-stu-id="251d9-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="251d9-121">เมื่อต้องการเข้าสู่เซฟโหมดหรือเปลี่ยนการตั้งค่าการเริ่มต้นขั้นสูงให้คลิก**แก้ไขปัญหา > ตัวเลือกขั้นสูง > การตั้งค่าการเริ่มต้น**แล้วคลิก**เริ่มใหม่**</span><span class="sxs-lookup"><span data-stu-id="251d9-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="251d9-122">คุณอาจถูกขอให้ใส่ [คีย์การกู้คืน BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)ของคุณ</span><span class="sxs-lookup"><span data-stu-id="251d9-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="251d9-123">หลังจากพีซีของคุณเริ่มระบบใหม่อีกครั้งให้คลิกการตั้งค่าการเริ่มต้นที่คุณต้องการใช้</span><span class="sxs-lookup"><span data-stu-id="251d9-123">After your PC restarts again, click the startup setting you want to use.</span></span>