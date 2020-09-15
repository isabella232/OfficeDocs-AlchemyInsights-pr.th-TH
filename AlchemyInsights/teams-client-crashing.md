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
# <a name="teams-client-crashing"></a>ไคลเอ็นต์ของทีมหยุดทำงานหรือไม่

ถ้าไคลเอ็นต์ทีมของคุณหยุดทำงานให้ลองทำดังต่อไปนี้:

- ถ้าคุณกำลังใช้แอปทีมบนเดสก์ท็อปให้ [ตรวจสอบให้แน่ใจว่าได้อัปเดตแอปที่สมบูรณ์](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)แล้ว

- ตรวจสอบให้แน่ใจว่าคุณสามารถเข้าถึง [url และช่วงที่อยู่ของ Microsoft ๓๖๕](https://docs.microsoft.com/microsoftteams/connectivity-issues) ทั้งหมดได้

- ลงชื่อเข้าใช้ด้วยบัญชีผู้ดูแลผู้เช่าของคุณและตรวจสอบ [แดชบอร์ดความสมบูรณ์ของบริการ](https://docs.microsoft.com/office365/enterprise/view-service-health) ของคุณเพื่อตรวจสอบว่าไม่มีกระแสตกหรือบริการที่มีการลดทอน

- ถอนการติดตั้งและติดตั้งแอปพลิเคชันของทีมใหม่ (ลิงก์)
    - เรียกดูโฟลเดอร์%appdata%\Microsoft\teams\ บนคอมพิวเตอร์ของคุณและลบไฟล์ทั้งหมดในไดเรกทอรีนั้น
    - [ดาวน์โหลดและติดตั้งแอปทีม](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)และถ้าเป็นไปได้ให้ติดตั้งทีมในฐานะผู้ดูแลระบบ (คลิกขวาที่ตัวติดตั้งทีมแล้วเลือก "เรียกใช้ในฐานะผู้ดูแลระบบ" ถ้าพร้อมใช้งาน)

ถ้าไคลเอ็นต์ทีมของคุณยังคงหยุดทำงานคุณสามารถทำซ้ำปัญหาได้หรือไม่ ถ้าเป็นเช่นนั้น:

1. ใช้ตัวบันทึกขั้นตอนเพื่อจับภาพขั้นตอนของคุณ
    - ปิดแอปพลิเคชันที่ไม่จำเป็นหรือเป็นความลับทั้งหมด
    - เปิดใช้งานตัวบันทึกขั้นตอนและทำซ้ำปัญหาในขณะที่เข้าสู่ระบบด้วยบัญชีผู้ใช้ที่ได้รับผลกระทบ
    - [รวบรวมบันทึกของทีมที่จับภาพขั้นตอนของ repro ที่บันทึกไว้](https://docs.microsoft.com/microsoftteams/log-files) **หมายเหตุ**: ตรวจสอบให้แน่ใจว่าคุณจับภาพที่อยู่การลงชื่อเข้าใช้ของผู้ใช้ที่ได้รับผลกระทบ
    - รวบรวมข้อมูลการถ่ายโอนข้อมูลและ/หรือข้อมูลกลุ่มข้อบกพร่อง (Windows) เปิดใช้งาน Windows Powershell บนเครื่องที่เกิดความผิดพลาดและเรียกใช้คำสั่งต่อไปนี้:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. แนบไฟล์ไปยังกรณีสนับสนุนของคุณ
