---
title: แก้ไขปัญหาการหยุดการหยุดการ OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826218"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="6e37a-102">แก้ไขปัญหาการหยุดการหยุดการ OneDrive</span><span class="sxs-lookup"><span data-stu-id="6e37a-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="6e37a-103">ถ้า OneDrive หยุดการเกิดขึ้นซ้ําๆ ให้ลองขั้นตอนการแก้ไขปัญหาเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="6e37a-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="6e37a-104">**ตรวจสอบให้แน่ใจว่าไม่ได้ตั้งค่ารีจิสทรีคีย์:**</span><span class="sxs-lookup"><span data-stu-id="6e37a-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="6e37a-105">ใช้ Registry Editor นําทางHKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="6e37a-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="6e37a-106">ถ้า DisableFileSyncNGSC แสดงอยู่และตั้งค่าเป็น 1 ให้เปิดคีย์และเปลี่ยนค่าเป็น 0</span><span class="sxs-lookup"><span data-stu-id="6e37a-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="6e37a-107">เปิดใช้ OneDrive ด้วยตนเอง โดยไปที่เริ่ม</span><span class="sxs-lookup"><span data-stu-id="6e37a-107">Manually launch OneDrive by going to Start</span></span> ![กดแป้น Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6e37a-109">พิมพ์ OneDrive ในกล่องค้นหา แล้วคลิกแอป OneDrive บนเดสก์ท็อป</span><span class="sxs-lookup"><span data-stu-id="6e37a-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6e37a-110">**รีเซ็ต OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="6e37a-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="6e37a-111">หมายเหตุ:</span><span class="sxs-lookup"><span data-stu-id="6e37a-111">Notes:</span></span>

- <span data-ttu-id="6e37a-112">การรีเซ็ต OneDrive จะยกเลิกการเชื่อมต่อการซิงค์ที่มีอยู่ของคุณทั้งหมด (รวมถึง OneDrive ส่วนบุคคลของคุณถ้าตั้งค่าไว้)</span><span class="sxs-lookup"><span data-stu-id="6e37a-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="6e37a-113">คุณจะไม่สูญเสียไฟล์หรือข้อมูลโดยการรีเซ็ต OneDrive บนคอมพิวเตอร์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="6e37a-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="6e37a-114">**เมื่อต้องการรีเซ็ต OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="6e37a-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="6e37a-115">เปิดกล่องโต้ตอบ เรียกใช้ โดยการกดแป้น Windows และ R</span><span class="sxs-lookup"><span data-stu-id="6e37a-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="6e37a-116">พิมพ์ %localappdata%\Microsoft\OneDrive\onedrive.exe /reset แล้วกด ตกลง</span><span class="sxs-lookup"><span data-stu-id="6e37a-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="6e37a-117">หน้าต่าง Command อาจปรากฏขึ้นสั้นๆ</span><span class="sxs-lookup"><span data-stu-id="6e37a-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="6e37a-118">เปิดใช้ OneDrive ด้วยตนเอง โดยไปที่เริ่ม</span><span class="sxs-lookup"><span data-stu-id="6e37a-118">Manually launch OneDrive by going to Start</span></span> ![กดแป้น Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6e37a-120">พิมพ์ OneDrive ในกล่องค้นหา แล้วคลิกแอป OneDrive บนเดสก์ท็อป</span><span class="sxs-lookup"><span data-stu-id="6e37a-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6e37a-121">หมายเหตุ:</span><span class="sxs-lookup"><span data-stu-id="6e37a-121">Notes:</span></span>

- <span data-ttu-id="6e37a-122">ถ้าคุณเลือกที่จะซิงค์เฉพาะบางโฟลเดอร์ก่อนการรีเซ็ต คุณจะต้องซิงค์อีกครั้งเมื่อการซิงค์เสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="6e37a-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="6e37a-123">อ่าน [เลือกโฟลเดอร์ OneDrive ที่คุณต้องการซิงค์กับคอมพิวเตอร์](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   ของคุณ เพื่อดูข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="6e37a-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="6e37a-124">คุณจะต้องเสร็จสิ้นการนี้กับ OneDrive ส่วนบุคคลของคุณและ OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="6e37a-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>