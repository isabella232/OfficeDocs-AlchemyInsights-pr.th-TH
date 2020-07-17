---
title: การแก้ไขปัญหาการหยุดทํางานของ OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749171"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="e863b-102">การแก้ไขปัญหาการหยุดทํางานของ OneDrive</span><span class="sxs-lookup"><span data-stu-id="e863b-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="e863b-103">หาก OneDrive ล้มเหลวซ้ํา ๆ ลองทําตามขั้นตอนการแก้ไขปัญหาเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="e863b-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="e863b-104">**ตรวจสอบให้แน่ใจว่าไม่ได้ตั้งค่ารีจิสทรีคีย์:**</span><span class="sxs-lookup"><span data-stu-id="e863b-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="e863b-105">การใช้ตัวแก้ไขรีจิสทรี ให้นําทางไปยัง HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="e863b-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="e863b-106">ถ้า DisableFileSyncNGSC อยู่ และตั้งค่าเป็น 1 เปิดคีย์ และเปลี่ยนค่าเป็น 0</span><span class="sxs-lookup"><span data-stu-id="e863b-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="e863b-107">เปิดใช้ OneDrive ด้วยตนเองโดยไปที่หน้าจอเริ่ม</span><span class="sxs-lookup"><span data-stu-id="e863b-107">Manually launch OneDrive by going to Start</span></span> ![กดแป้น Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="e863b-109">ประเภท:OneDriveในกล่องค้นหา แล้วคลิกบนแอป OneDrive เดสก์ท็อป</span><span class="sxs-lookup"><span data-stu-id="e863b-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="e863b-110">**รีเซ็ต OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="e863b-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="e863b-111">หมาย เหตุ:</span><span class="sxs-lookup"><span data-stu-id="e863b-111">Notes:</span></span>

- <span data-ttu-id="e863b-112">การรีเซ็ต OneDrive จะยกเลิกการเชื่อมต่อการซิงค์ทั้งหมดที่มีอยู่ (รวมถึง OneDrive ส่วนบุคคลของคุณถ้าตั้งค่า)</span><span class="sxs-lookup"><span data-stu-id="e863b-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="e863b-113">คุณจะไม่สูญเสียไฟล์หรือข้อมูลด้วยการรีเซ็ต OneDrive บนคอมพิวเตอร์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="e863b-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="e863b-114">**เมื่อต้องการรีเซ็ต OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="e863b-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="e863b-115">เปิดกล่องโต้ตอบเรียกใช้โดยการกดแป้น Windows และ R</span><span class="sxs-lookup"><span data-stu-id="e863b-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="e863b-116">พิมพ์ %localappdata%\Microsoft\OneDrive\onedrive.exe /reset และกด ตกลง</span><span class="sxs-lookup"><span data-stu-id="e863b-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="e863b-117">หน้าต่างคําสั่งอาจปรากฏขึ้นสั้น ๆ</span><span class="sxs-lookup"><span data-stu-id="e863b-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="e863b-118">เปิดใช้ OneDrive ด้วยตนเองโดยไปที่หน้าจอเริ่ม</span><span class="sxs-lookup"><span data-stu-id="e863b-118">Manually launch OneDrive by going to Start</span></span> ![กดแป้น Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="e863b-120">ประเภท:OneDriveในกล่องค้นหา แล้วคลิกบนแอป OneDrive เดสก์ท็อป</span><span class="sxs-lookup"><span data-stu-id="e863b-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="e863b-121">หมาย เหตุ:</span><span class="sxs-lookup"><span data-stu-id="e863b-121">Notes:</span></span>

- <span data-ttu-id="e863b-122">หากคุณเลือกที่จะซิงค์เฉพาะบางโฟลเดอร์ก่อนการตั้งค่าใหม่ คุณจะต้องทําอีกครั้งเมื่อซิงค์เสร็จสิ้น</span><span class="sxs-lookup"><span data-stu-id="e863b-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="e863b-123">อ่าน [เลือกโฟลเดอร์ OneDrive ที่จะซิงค์กับคอมพิวเตอร์ของคุณ](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="e863b-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="e863b-124">คุณจะต้องดําเนินการนี้ให้เสร็จสมบูรณ์สําหรับ OneDrive ส่วนบุคคลของคุณและ OneDrive สําหรับธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="e863b-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>