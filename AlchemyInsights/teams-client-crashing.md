---
title: ไคลเอ็นต์ของทีมหยุดทำงานหรือไม่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691126"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="f75a7-102">ไคลเอ็นต์ของทีมหยุดทำงานหรือไม่</span><span class="sxs-lookup"><span data-stu-id="f75a7-102">Teams client crashing?</span></span>

<span data-ttu-id="f75a7-103">ถ้าไคลเอ็นต์ทีมของคุณหยุดทำงานให้ลองทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="f75a7-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="f75a7-104">ถ้าคุณกำลังใช้แอปทีมบนเดสก์ท็อปให้ [ตรวจสอบให้แน่ใจว่าได้อัปเดตแอปที่สมบูรณ์](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)แล้ว</span><span class="sxs-lookup"><span data-stu-id="f75a7-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="f75a7-105">ตรวจสอบให้แน่ใจว่าคุณสามารถเข้าถึง [url และช่วงที่อยู่ของ Microsoft ๓๖๕](https://docs.microsoft.com/microsoftteams/connectivity-issues) ทั้งหมดได้</span><span class="sxs-lookup"><span data-stu-id="f75a7-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="f75a7-106">ลงชื่อเข้าใช้ด้วยบัญชีผู้ดูแลผู้เช่าของคุณและตรวจสอบ [แดชบอร์ดความสมบูรณ์ของบริการ](https://docs.microsoft.com/office365/enterprise/view-service-health) ของคุณเพื่อตรวจสอบว่าไม่มีกระแสตกหรือบริการที่มีการลดทอน</span><span class="sxs-lookup"><span data-stu-id="f75a7-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="f75a7-107">ถอนการติดตั้งและติดตั้งแอปพลิเคชันของทีมใหม่ (ลิงก์)</span><span class="sxs-lookup"><span data-stu-id="f75a7-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="f75a7-108">เรียกดูโฟลเดอร์%appdata%\Microsoft\teams\ บนคอมพิวเตอร์ของคุณและลบไฟล์ทั้งหมดในไดเรกทอรีนั้น</span><span class="sxs-lookup"><span data-stu-id="f75a7-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="f75a7-109">[ดาวน์โหลดและติดตั้งแอปทีม](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)และถ้าเป็นไปได้ให้ติดตั้งทีมในฐานะผู้ดูแลระบบ (คลิกขวาที่ตัวติดตั้งทีมแล้วเลือก "เรียกใช้ในฐานะผู้ดูแลระบบ" ถ้าพร้อมใช้งาน)</span><span class="sxs-lookup"><span data-stu-id="f75a7-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="f75a7-110">ถ้าไคลเอ็นต์ทีมของคุณยังคงหยุดทำงานคุณสามารถทำซ้ำปัญหาได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="f75a7-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="f75a7-111">ถ้าเป็นเช่นนั้น:</span><span class="sxs-lookup"><span data-stu-id="f75a7-111">If so:</span></span>

1. <span data-ttu-id="f75a7-112">ใช้ตัวบันทึกขั้นตอนเพื่อจับภาพขั้นตอนของคุณ</span><span class="sxs-lookup"><span data-stu-id="f75a7-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="f75a7-113">ปิดแอปพลิเคชันที่ไม่จำเป็นหรือเป็นความลับทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="f75a7-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="f75a7-114">เปิดใช้งานตัวบันทึกขั้นตอนและทำซ้ำปัญหาในขณะที่เข้าสู่ระบบด้วยบัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="f75a7-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="f75a7-115">[รวบรวมบันทึกของทีมที่จับภาพขั้นตอนของ repro ที่บันทึกไว้](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="f75a7-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="f75a7-116">**หมายเหตุ**: ตรวจสอบให้แน่ใจว่าคุณจับภาพที่อยู่การลงชื่อเข้าใช้ของผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="f75a7-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="f75a7-117">รวบรวมข้อมูลการถ่ายโอนข้อมูลและ/หรือข้อมูลกลุ่มข้อบกพร่อง (Windows)</span><span class="sxs-lookup"><span data-stu-id="f75a7-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="f75a7-118">เปิดใช้งาน Windows Powershell บนเครื่องที่เกิดความผิดพลาดและเรียกใช้คำสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="f75a7-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="f75a7-119">แนบไฟล์ไปยังกรณีสนับสนุนของคุณ</span><span class="sxs-lookup"><span data-stu-id="f75a7-119">Attach the file to your support case.</span></span>
