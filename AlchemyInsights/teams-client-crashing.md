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
# <a name="teams-client-crashing"></a>ลูกค้าทีมล้มเหลว?

หากไคลเอ็นต์ Teams ของคุณหยุดทํางาน ให้ลองทําดังต่อไปนี้

- ถ้าคุณกําลังใช้แอปทีมบนเดสก์ท็อป ให้ตรวจสอบ[ให้แน่ใจว่าแอปได้รับการอัปเดตอย่างสมบูรณ์](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)แล้ว

- ตรวจสอบให้แน่ใจว่าสามารถเข้าถึง[URL และช่วงที่อยู่ของ Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues)ทั้งหมดได้

- เข้าสู่ระบบด้วยบัญชีผู้ดูแลระบบผู้เช่าของคุณ และตรวจสอบ[แดชบอร์ดสถานภาพบริการ](https://docs.microsoft.com/office365/enterprise/view-service-health)ของคุณเพื่อตรวจสอบว่าไม่มีการเสื่อมสภาพหรือการบริการ

- ถอนการติดตั้งและติดตั้งแอพลิเคชันของทีม (ลิงค์)
    - เรียกดูโฟลเดอร์ %appdata%\Microsoft\teams\ บนคอมพิวเตอร์ของคุณและลบไฟล์ทั้งหมดในไดเรกทอรีนั้น
    - [ดาวน์โหลดและติดตั้งแอป Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)และถ้าเป็นไปได้ ให้ติดตั้ง Teams ในฐานะผู้ดูแลระบบ (คลิกขวาที่ตัวติดตั้ง Teams และเลือก "เรียกใช้ในฐานะผู้ดูแลระบบ" หากมี)

หากไคลเอ็นต์ Teams ของคุณยังคงหยุดทํางาน คุณสามารถทบทวนปัญหาได้หรือไม่ ถ้าเป็นเช่นนั้น:

1. ใช้ตัวบันทึกขั้นตอนเพื่อจับภาพขั้นตอนของคุณ
    - ปิดโปรแกรมประยุกต์ที่ไม่จําเป็นหรือเป็นความลับทั้งหมด
    - เปิดตัวตัวบันทึกขั้นตอน และทบทวนเกิดปัญหาในขณะที่เข้าสู่ระบบด้วยบัญชีผู้ใช้ที่ได้รับผลกระทบ
    - [รวบรวมบันทึกของทีมที่จับภาพขั้นตอน repro ที่บันทึกไว้](https://docs.microsoft.com/microsoftteams/log-files) **หมายเหตุ**: ตรวจสอบให้แน่ใจว่าคุณได้บันทึกที่อยู่การลงชื่อเข้าใช้ของผู้ใช้ที่ได้รับผลกระทบ
    - เก็บรวบรวมการถ่ายโอนข้อมูลและ/หรือข้อมูลบัคเก็ตข้อบกพร่อง (Windows) เปิดใช้ Windows Powershell บนเครื่องที่เกิดความผิดพลาด และเรียกใช้คําสั่งต่อไปนี้:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. แนบไฟล์เข้ากับกรณีการสนับสนุนของคุณ
