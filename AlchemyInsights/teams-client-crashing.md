---
title: ลูกค้าทีมล้มเหลว?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: c49dfbf422b312f4744711d5f12b0eb83b6ebf2e
ms.sourcegitcommit: b398afd92d4259f893c25b48aec65921e6cc68d6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/16/2020
ms.locfileid: "44268791"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="38e27-102">ลูกค้าทีมล้มเหลว?</span><span class="sxs-lookup"><span data-stu-id="38e27-102">Teams client crashing?</span></span>

<span data-ttu-id="38e27-103">หากไคลเอ็นต์ Teams ของคุณหยุดทํางาน ให้ลองทําดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="38e27-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="38e27-104">ถ้าคุณกําลังใช้แอปทีมบนเดสก์ท็อป ให้ตรวจสอบ[ให้แน่ใจว่าแอปได้รับการอัปเดตอย่างสมบูรณ์](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)แล้ว</span><span class="sxs-lookup"><span data-stu-id="38e27-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="38e27-105">ตรวจสอบให้แน่ใจว่าสามารถเข้าถึง[URL และช่วงที่อยู่ของ Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues)ทั้งหมดได้</span><span class="sxs-lookup"><span data-stu-id="38e27-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="38e27-106">เข้าสู่ระบบด้วยบัญชีผู้ดูแลระบบผู้เช่าของคุณ และตรวจสอบ[แดชบอร์ดสถานภาพบริการ](https://docs.microsoft.com/office365/enterprise/view-service-health)ของคุณเพื่อตรวจสอบว่าไม่มีการเสื่อมสภาพหรือการบริการ</span><span class="sxs-lookup"><span data-stu-id="38e27-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="38e27-107">ขั้นตอนสุดท้าย คุณสามารถพยายามล้างแคชของไคลเอ็นต์ Teams ของคุณ:</span><span class="sxs-lookup"><span data-stu-id="38e27-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="38e27-108">ออกจากไคลเอ็นต์เดสก์ท็อปทีม Microsoft อย่างสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="38e27-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="38e27-109">คุณสามารถคลิกขวาที่**ทีม**จากถาดไอคอน และคลิก**ออก**หรือเรียกใช้ตัวจัดการงาน และฆ่ากระบวนการทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="38e27-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="38e27-110">ไปที่ File Explorer แล้วพิมพ์ข้อมูล %Microsoft\ทีม</span><span class="sxs-lookup"><span data-stu-id="38e27-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="38e27-111">เมื่ออยู่ในไดเรกทอรีคุณจะเห็นโฟลเดอร์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="38e27-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="38e27-112">จากภายใน**แคชแอพลิเคชัน**ไปที่แคชและลบไฟล์ใด ๆ ในแคชที่ตั้ง: %appdata%\Microsoft \ทีมงาน \ แคชใบสมัคร</span><span class="sxs-lookup"><span data-stu-id="38e27-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="38e27-113">จาก**ภายในBlob_storage**ลบแฟ้มทั้งหมด: %appdata%\Microsoft\ทีม\blob_storage</span><span class="sxs-lookup"><span data-stu-id="38e27-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="38e27-114">จากภายใน**แคช**ลบไฟล์ทั้งหมด: %appdata%\ทีม\แคช</span><span class="sxs-lookup"><span data-stu-id="38e27-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="38e27-115">จาก**ภายในฐานข้อมูล**ลบแฟ้มทั้งหมด: %appdata%\Microsoft\ทีม\ฐานข้อมูล</span><span class="sxs-lookup"><span data-stu-id="38e27-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="38e27-116">จากภายใน**GPUCache**ลบไฟล์ทั้งหมด: %appdata%\ทีม\GPUcache</span><span class="sxs-lookup"><span data-stu-id="38e27-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="38e27-117">จากภายใน**ดัชนี DB**ให้ลบแฟ้ม .db: %appdata%\Microsoft\ทีม\ทําดัชนีDB</span><span class="sxs-lookup"><span data-stu-id="38e27-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="38e27-118">จาก**ภายในที่เก็บภายใน**ให้ลบแฟ้มทั้งหมด: %appdata%\Microsoft\teams\ที่เก็บข้อมูลภายในเครื่อง</span><span class="sxs-lookup"><span data-stu-id="38e27-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="38e27-119">สุดท้ายจากภายใน**tmp**ลบไฟล์ใด ๆ: %appdata%\ทีม\ทีม\tmp</span><span class="sxs-lookup"><span data-stu-id="38e27-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="38e27-120">รีสตาร์ทไคลเอนต์ Teams ของคุณ</span><span class="sxs-lookup"><span data-stu-id="38e27-120">Restart your Teams client.</span></span>

<span data-ttu-id="38e27-121">หากไคลเอ็นต์ Teams ของคุณยังคงหยุดทํางาน คุณสามารถทบทวนปัญหาได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="38e27-121">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="38e27-122">ถ้าเป็นเช่นนั้น:</span><span class="sxs-lookup"><span data-stu-id="38e27-122">If so:</span></span> 

1. <span data-ttu-id="38e27-123">ใช้ตัวบันทึกขั้นตอนเพื่อจับภาพขั้นตอนของคุณ</span><span class="sxs-lookup"><span data-stu-id="38e27-123">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="38e27-124">ปิดโปรแกรมประยุกต์ที่ไม่จําเป็นหรือเป็นความลับทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="38e27-124">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="38e27-125">เปิดตัวตัวบันทึกขั้นตอน และทบทวนเกิดปัญหาในขณะที่เข้าสู่ระบบด้วยบัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="38e27-125">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    
2. <span data-ttu-id="38e27-126">แนบไฟล์เข้ากับกรณีการสนับสนุนของคุณ</span><span class="sxs-lookup"><span data-stu-id="38e27-126">Attach the file to your support case.</span></span>
