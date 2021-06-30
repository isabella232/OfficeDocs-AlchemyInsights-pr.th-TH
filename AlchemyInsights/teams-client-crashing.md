---
title: Teamsไคลเอ็นต์หยุดการหยุด
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187740"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="e534c-102">Teamsไคลเอ็นต์หยุดการหยุด</span><span class="sxs-lookup"><span data-stu-id="e534c-102">Teams client crashing</span></span>

<span data-ttu-id="e534c-103">ถ้าไคลเอ็นต์ Teamsของคุณหยุดการหยุดให้บริการ ให้ลองวิธีต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e534c-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="e534c-104">ถ้าคุณใช้แอป Teams บนเดสก์ท็อป[ตรวจสอบให้แน่ใจว่าแอปได้รับการอัปเดต](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)อย่างสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="e534c-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="e534c-105">ตรวจสอบให้แน่ใจว่า[URL Microsoft 365และช่วงที่อยู่ทั้งหมด](/microsoftteams/connectivity-issues)สามารถเข้าถึงได้</span><span class="sxs-lookup"><span data-stu-id="e534c-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="e534c-106">เข้าสู่ระบบด้วยบัญชีผู้ดูแลระบบผู้เช่าของคุณ และตรวจสอบ [แดชบอร์ดสถาน](/office365/enterprise/view-service-health) ภาพบริการของคุณเพื่อตรวจสอบว่าไม่มีข้อมูลการไม่อยู่หรือการลดบริการ</span><span class="sxs-lookup"><span data-stu-id="e534c-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="e534c-107">ถอนการติดตั้งและติดตั้งแอปพลิเคชัน Teams อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="e534c-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="e534c-108">เรียกดูโฟลเดอร์ %appdata%\Microsoft\Teams\ บนคอมพิวเตอร์ของคุณ แล้วลบไฟล์ทั้งหมดในไดเรกทอรีนั้น</span><span class="sxs-lookup"><span data-stu-id="e534c-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="e534c-109">[ดาวน์โหลดและติดตั้งแอป Teams และ](https://www.microsoft.com/microsoft-teams/download-app)ถ้าเป็นไปได้ ให้ติดตั้ง Teams ในฐานะผู้ดูแลระบบ (คลิกขวาที่ตัวติดตั้ง Teams และเลือก **เรียกใช้** ในฐานะผู้ดูแลระบบ ถ้ามี)</span><span class="sxs-lookup"><span data-stu-id="e534c-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="e534c-110">ถ้าไคลเอ็นต์ Teamsของคุณยังคงหยุดการเกิดขึ้น ให้ลองให้เกิดปัญหานี้อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="e534c-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="e534c-111">ถ้าคุณสามารถ:</span><span class="sxs-lookup"><span data-stu-id="e534c-111">If you can:</span></span>

1. <span data-ttu-id="e534c-112">ใช้ตัวบันทึกขั้นตอนเพื่อบันทึกขั้นตอนของคุณ</span><span class="sxs-lookup"><span data-stu-id="e534c-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="e534c-113">ปิดแอปพลิเคชันทั้งหมดโดยไม่จําเป็นหรือเป็นความลับ</span><span class="sxs-lookup"><span data-stu-id="e534c-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="e534c-114">เรียกใช้ตัวบันทึกขั้นตอน และพบปัญหาขณะเข้าสู่ระบบด้วยบัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="e534c-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="e534c-115">[รวบรวมบันทึกของทีมที่บันทึกขั้นตอน repro ที่บันทึกไว้](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="e534c-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="e534c-116">**หมายเหตุ**: ตรวจสอบให้แน่ใจว่าคุณบันทึกที่อยู่การลงชื่อเข้าใช้ของผู้ใช้ที่มีผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="e534c-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="e534c-117">รวบรวมข้อมูลการเก็บและ/หรือข้อมูลกลุ่มความผิดพลาด (Windows)</span><span class="sxs-lookup"><span data-stu-id="e534c-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="e534c-118">เรียกใช้Windows Powershell บนเครื่องที่ระบบหยุดการหยุดและเรียกใช้สั่งต่อไปนี้ (หลังจากแต่ละสั่ง ให้กด Enter):</span><span class="sxs-lookup"><span data-stu-id="e534c-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="e534c-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="e534c-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="e534c-120">หลังจากไฟล์ข้อความถูกสร้างขึ้นและปรากฏบนหน้าจอของคุณ ให้บันทึกไฟล์และแนบไฟล์ลงในการร้องขอบริการ</span><span class="sxs-lookup"><span data-stu-id="e534c-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
