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
# <a name="teams-client-crashing"></a>ลูกค้า Teams หยุดการใช่หรือเปล่า

ถ้าไคลเอ็นต์ Teams ของคุณหยุดการผิดพลาด ให้ลองวิธีต่อไปนี้:

- ถ้าคุณใช้แอป Teams บนเดสก์ท็อป [ตรวจสอบให้แน่ใจว่าแอปได้รับการอัปเดต](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)เต็มรูปแบบ

- ตรวจสอบให้แน่ใจว่า URL [และช่วงที่อยู่ของ Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) ทั้งหมดสามารถเข้าถึงได้

- เข้าสู่ระบบด้วยบัญชีผู้ดูแลระบบผู้เช่าของคุณ และตรวจสอบ [แดชบอร์ดสถาน](https://docs.microsoft.com/office365/enterprise/view-service-health) ภาพบริการของคุณเพื่อตรวจสอบว่าไม่มีข้อมูลการไม่อยู่หรือการลดบริการ

- ถอนการติดตั้งและติดตั้งแอปพลิเคชัน Teams ใหม่ (ลิงก์)
    - เรียกดูโฟลเดอร์ %appdata%\Microsoft\teams\ บนคอมพิวเตอร์ของคุณ แล้วลบไฟล์ทั้งหมดในไดเรกทอรีนั้น
    - [ดาวน์โหลดและติดตั้งแอป Teams และ](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)ถ้าเป็นไปได้ ให้ติดตั้ง Teams ในฐานะผู้ดูแลระบบ (คลิกขวาที่ตัวติดตั้ง Teams และเลือก "เรียกใช้ในฐานะผู้ดูแลระบบ" ถ้ามี)

ถ้าไคลเอ็นต์ Teams ของคุณยังคงหยุดการหยุดการใช่ คุณสามารถให้เกิดปัญหานั้นขึ้นได้หรือไม่ หากเป็นดังนั้น:

1. ใช้ตัวบันทึกขั้นตอนเพื่อบันทึกขั้นตอนของคุณ
    - ปิดแอปพลิเคชันทั้งหมดโดยไม่จําเป็นหรือเป็นความลับ
    - เรียกใช้ตัวบันทึกขั้นตอน และพบปัญหาขณะเข้าสู่ระบบด้วยบัญชีผู้ใช้ที่ได้รับผลกระทบ
    - [รวบรวมบันทึกของทีมที่บันทึกขั้นตอน repro ที่บันทึกไว้](https://docs.microsoft.com/microsoftteams/log-files) **หมายเหตุ**: ตรวจสอบให้แน่ใจว่าคุณบันทึกที่อยู่การลงชื่อเข้าใช้ของผู้ใช้ที่มีผลกระทบ
    - รวบรวมข้อมูลการเก็บและ/หรือข้อมูลกลุ่มความผิดพลาด (Windows) เปิดใช้ Windows Powershell บนเครื่องที่ระบบหยุดการหยุดการหยุดและเรียกใช้การสั่งต่อไปนี้:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. แนบไฟล์กับกรณีการสนับสนุนของคุณ
