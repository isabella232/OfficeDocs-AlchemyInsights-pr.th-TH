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
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354072"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="397ed-102">ลูกค้าทีมล้มเหลว?</span><span class="sxs-lookup"><span data-stu-id="397ed-102">Teams client crashing?</span></span>

<span data-ttu-id="397ed-103">หากไคลเอ็นต์ Teams ของคุณหยุดทํางาน ให้ลองทําดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="397ed-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="397ed-104">ถ้าคุณกําลังใช้แอปทีมบนเดสก์ท็อป ให้ตรวจสอบ[ให้แน่ใจว่าแอปได้รับการอัปเดตอย่างสมบูรณ์](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)แล้ว</span><span class="sxs-lookup"><span data-stu-id="397ed-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="397ed-105">ตรวจสอบให้แน่ใจว่าสามารถเข้าถึง[URL และช่วงที่อยู่ของ Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues)ทั้งหมดได้</span><span class="sxs-lookup"><span data-stu-id="397ed-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="397ed-106">เข้าสู่ระบบด้วยบัญชีผู้ดูแลระบบผู้เช่าของคุณ และตรวจสอบ[แดชบอร์ดสถานภาพบริการ](https://docs.microsoft.com/office365/enterprise/view-service-health)ของคุณเพื่อตรวจสอบว่าไม่มีการเสื่อมสภาพหรือการบริการ</span><span class="sxs-lookup"><span data-stu-id="397ed-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="397ed-107">ถอนการติดตั้งและติดตั้งแอพลิเคชันของทีม (ลิงค์)</span><span class="sxs-lookup"><span data-stu-id="397ed-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="397ed-108">เรียกดูโฟลเดอร์ %appdata%\Microsoft\teams\ บนคอมพิวเตอร์ของคุณและลบไฟล์ทั้งหมดในไดเรกทอรีนั้น</span><span class="sxs-lookup"><span data-stu-id="397ed-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="397ed-109">[ดาวน์โหลดและติดตั้งแอป Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)และถ้าเป็นไปได้ ให้ติดตั้ง Teams ในฐานะผู้ดูแลระบบ (คลิกขวาที่ตัวติดตั้ง Teams และเลือก "เรียกใช้ในฐานะผู้ดูแลระบบ" หากมี)</span><span class="sxs-lookup"><span data-stu-id="397ed-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="397ed-110">หากไคลเอ็นต์ Teams ของคุณยังคงหยุดทํางาน คุณสามารถทบทวนปัญหาได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="397ed-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="397ed-111">ถ้าเป็นเช่นนั้น:</span><span class="sxs-lookup"><span data-stu-id="397ed-111">If so:</span></span>

1. <span data-ttu-id="397ed-112">ใช้ตัวบันทึกขั้นตอนเพื่อจับภาพขั้นตอนของคุณ</span><span class="sxs-lookup"><span data-stu-id="397ed-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="397ed-113">ปิดโปรแกรมประยุกต์ที่ไม่จําเป็นหรือเป็นความลับทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="397ed-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="397ed-114">เปิดตัวตัวบันทึกขั้นตอน และทบทวนเกิดปัญหาในขณะที่เข้าสู่ระบบด้วยบัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="397ed-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="397ed-115">[รวบรวมบันทึกของทีมที่จับภาพขั้นตอน repro ที่บันทึกไว้](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="397ed-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="397ed-116">**หมายเหตุ**: ตรวจสอบให้แน่ใจว่าคุณได้บันทึกที่อยู่การลงชื่อเข้าใช้ของผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="397ed-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="397ed-117">เก็บรวบรวมการถ่ายโอนข้อมูลและ/หรือข้อมูลบัคเก็ตข้อบกพร่อง (Windows)</span><span class="sxs-lookup"><span data-stu-id="397ed-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="397ed-118">เปิดใช้ Windows Powershell บนเครื่องที่เกิดความผิดพลาด และเรียกใช้คําสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="397ed-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="397ed-119">แนบไฟล์เข้ากับกรณีการสนับสนุนของคุณ</span><span class="sxs-lookup"><span data-stu-id="397ed-119">Attach the file to your support case.</span></span>
