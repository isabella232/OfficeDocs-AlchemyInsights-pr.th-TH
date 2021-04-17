---
title: ลูกค้า Teams หยุดการใช่หรือเปล่า
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826290"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="da4f8-102">ลูกค้า Teams หยุดการใช่หรือเปล่า</span><span class="sxs-lookup"><span data-stu-id="da4f8-102">Teams client crashing?</span></span>

<span data-ttu-id="da4f8-103">ถ้าไคลเอ็นต์ Teams ของคุณหยุดการผิดพลาด ให้ลองวิธีต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="da4f8-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="da4f8-104">ถ้าคุณใช้แอป Teams บนเดสก์ท็อป [ตรวจสอบให้แน่ใจว่าแอปได้รับการอัปเดต](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)เต็มรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="da4f8-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="da4f8-105">ตรวจสอบให้แน่ใจว่า URL [และช่วงที่อยู่ของ Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) ทั้งหมดสามารถเข้าถึงได้</span><span class="sxs-lookup"><span data-stu-id="da4f8-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="da4f8-106">เข้าสู่ระบบด้วยบัญชีผู้ดูแลระบบผู้เช่าของคุณ และตรวจสอบ [แดชบอร์ดสถาน](https://docs.microsoft.com/office365/enterprise/view-service-health) ภาพบริการของคุณเพื่อตรวจสอบว่าไม่มีข้อมูลการไม่อยู่หรือการลดบริการ</span><span class="sxs-lookup"><span data-stu-id="da4f8-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="da4f8-107">ถอนการติดตั้งและติดตั้งแอปพลิเคชัน Teams ใหม่ (ลิงก์)</span><span class="sxs-lookup"><span data-stu-id="da4f8-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="da4f8-108">เรียกดูโฟลเดอร์ %appdata%\Microsoft\teams\ บนคอมพิวเตอร์ของคุณ แล้วลบไฟล์ทั้งหมดในไดเรกทอรีนั้น</span><span class="sxs-lookup"><span data-stu-id="da4f8-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="da4f8-109">[ดาวน์โหลดและติดตั้งแอป Teams และ](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)ถ้าเป็นไปได้ ให้ติดตั้ง Teams ในฐานะผู้ดูแลระบบ (คลิกขวาที่ตัวติดตั้ง Teams และเลือก "เรียกใช้ในฐานะผู้ดูแลระบบ" ถ้ามี)</span><span class="sxs-lookup"><span data-stu-id="da4f8-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="da4f8-110">ถ้าไคลเอ็นต์ Teams ของคุณยังคงหยุดการหยุดการใช่ คุณสามารถให้เกิดปัญหานั้นขึ้นได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="da4f8-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="da4f8-111">หากเป็นดังนั้น:</span><span class="sxs-lookup"><span data-stu-id="da4f8-111">If so:</span></span>

1. <span data-ttu-id="da4f8-112">ใช้ตัวบันทึกขั้นตอนเพื่อบันทึกขั้นตอนของคุณ</span><span class="sxs-lookup"><span data-stu-id="da4f8-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="da4f8-113">ปิดแอปพลิเคชันทั้งหมดโดยไม่จําเป็นหรือเป็นความลับ</span><span class="sxs-lookup"><span data-stu-id="da4f8-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="da4f8-114">เรียกใช้ตัวบันทึกขั้นตอน และพบปัญหาขณะเข้าสู่ระบบด้วยบัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="da4f8-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="da4f8-115">[รวบรวมบันทึกของทีมที่บันทึกขั้นตอน repro ที่บันทึกไว้](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="da4f8-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="da4f8-116">**หมายเหตุ**: ตรวจสอบให้แน่ใจว่าคุณบันทึกที่อยู่การลงชื่อเข้าใช้ของผู้ใช้ที่มีผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="da4f8-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="da4f8-117">รวบรวมข้อมูลการเก็บและ/หรือข้อมูลกลุ่มความผิดพลาด (Windows)</span><span class="sxs-lookup"><span data-stu-id="da4f8-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="da4f8-118">เปิดใช้ Windows Powershell บนเครื่องที่ระบบหยุดการหยุดการหยุดและเรียกใช้การสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="da4f8-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="da4f8-119">แนบไฟล์กับกรณีการสนับสนุนของคุณ</span><span class="sxs-lookup"><span data-stu-id="da4f8-119">Attach the file to your support case.</span></span>
