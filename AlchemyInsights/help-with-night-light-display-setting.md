---
title: ความช่วยเหลือเกี่ยวกับการตั้งค่าจอแสดงผลกลางคืน
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405183"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="f7e4d-102">ความช่วยเหลือเกี่ยวกับการตั้งค่าจอแสดงผลกลางคืน</span><span class="sxs-lookup"><span data-stu-id="f7e4d-102">Help with the night light display setting</span></span>

<span data-ttu-id="f7e4d-103">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการตั้งค่าการแสดงเวลากลางคืน ให้ดู[ตั้งค่าจอแสดงผลของคุณในช่วงเวลากลางคืนใน Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="f7e4d-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="f7e4d-104">หากตัวเลือกแสงกลางคืนเป็นสีเทาในการตั้งค่า ให้ตรวจสอบโปรแกรมควบคุมจอแสดงผลของคุณ:</span><span class="sxs-lookup"><span data-stu-id="f7e4d-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="f7e4d-105">คลิกกล่องค้นหาบนแถบงานของคุณ **แล้ว** พิมพ์ ตัวจัดการอุปกรณ์ แล้วเลือก **ตัวจัดการ** อุปกรณ์ ในผลลัพธ์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="f7e4d-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="f7e4d-106">ขยาย **การ์ดแสดงผล**</span><span class="sxs-lookup"><span data-stu-id="f7e4d-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="f7e4d-107">น่าเสียดายที่คุณลักษณะแสงกลางคืนไม่พร้อมใช้งานหากอุปกรณ์ของคุณใช้โปรแกรมควบคุม DisplayLink หรือโปรแกรมควบคุมจอแสดงผลพื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="f7e4d-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="f7e4d-108">ฟีเจอร์แสงกลางคืนจะใช้เทคโนโลยีกราฟิกล่าสุด ดังนั้นคุณอาจต้องอัปเดตโปรแกรมควบคุมจอแสดงผลของคุณ:</span><span class="sxs-lookup"><span data-stu-id="f7e4d-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="f7e4d-109">ตรวจหาการอัปเดตโดยไปที่ เริ่ม  >  **การอัปเดต**  >  **การตั้งค่า &ตรวจสอบ**  >    >  **การอัปเดตของ** Windows Security</span><span class="sxs-lookup"><span data-stu-id="f7e4d-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="f7e4d-110">OR</span><span class="sxs-lookup"><span data-stu-id="f7e4d-110">OR</span></span>

- <span data-ttu-id="f7e4d-111">เยี่ยมชมเว็บไซต์การสนับสนุนของผู้ผลิตฮาร์ดแวร์ของคุณเพื่อดาวน์โหลดและติดตั้งโปรแกรมควบคุมจอแสดงผลล่าสุดด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="f7e4d-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="f7e4d-112">รีเซ็ตแสงกลางคืนในรีจิสทรี</span><span class="sxs-lookup"><span data-stu-id="f7e4d-112">Reset night light in the registry</span></span>

<span data-ttu-id="f7e4d-113">หากการอัปเดตโปรแกรมควบคุมจอแสดงผลของคุณไม่ได้ผล คุณอาจต้องรีเซ็ตแสงกลางคืนในรีจิสทรี</span><span class="sxs-lookup"><span data-stu-id="f7e4d-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="f7e4d-114">**ข้อควรระวัง:** แนะนนะวิธีนี้เฉพาะผู้ใช้ขั้นสูง</span><span class="sxs-lookup"><span data-stu-id="f7e4d-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="f7e4d-115">ปัญหาร้ายแรงอาจเกิดขึ้นถ้าคุณปรับเปลี่ยนรีจิสทรีอย่างไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="f7e4d-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="f7e4d-116">เมื่อต้องการป้องกันเพิ่มเติม ให้ย้อนกลับรีจิสทรีก่อนที่คุณจะปรับเปลี่ยน เพื่อให้คุณสามารถคืนค่าได้ถ้ามีปัญหาเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="f7e4d-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="f7e4d-117">ในกล่องค้นหา ให้พิมพ์ **regedit** แล้วเลือก Registry **Editor** ในผลลัพธ์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="f7e4d-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="f7e4d-118">ไปที่คีย์รีจิสทรีต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="f7e4d-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="f7e4d-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="f7e4d-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="f7e4d-120">ส่งออก และลบซับคีย์ต่อไปนี้:$$windows.data.bluelightreduction.bluelightreductionstated</span><span class="sxs-lookup"><span data-stu-id="f7e4d-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="f7e4d-121">ส่งออก และลบซับคีย์ต่อไปนี้:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="f7e4d-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="f7e4d-122">รีสตาร์ต Windows และตรวจสอบว่ามีตัวเลือกแสงกลางคืนพร้อมใช้งานหรือไม่</span><span class="sxs-lookup"><span data-stu-id="f7e4d-122">Restart Windows and verify if the night light options are available.</span></span>


