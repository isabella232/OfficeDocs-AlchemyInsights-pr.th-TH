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
ms.openlocfilehash: bef16351b55ac4765539d66ab86a71183f66f0dd
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321644"
---
# <a name="teams-client-crashing"></a>Teamsไคลเอ็นต์หยุดการหยุด

ถ้าไคลเอ็นต์ Teamsของคุณหยุดการหยุดให้บริการ ให้ลองวิธีต่อไปนี้:

- ถ้าคุณใช้งาน Teams แอป[บนเดสก์ท็อป ตรวจสอบให้แน่ใจว่าแอปได้รับการอัปเดต](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)อย่างสมบูรณ์

- ตรวจสอบให้แน่ใจว่า[URL Microsoft 365และช่วงที่อยู่ทั้งหมด](https://docs.microsoft.com/microsoftteams/connectivity-issues)สามารถเข้าถึงได้

- เข้าสู่ระบบด้วยบัญชีผู้ดูแลระบบผู้เช่าของคุณ และตรวจสอบ [แดชบอร์ดสถาน](https://docs.microsoft.com/office365/enterprise/view-service-health) ภาพบริการของคุณเพื่อตรวจสอบว่าไม่มีข้อมูลการไม่อยู่หรือการลดบริการ

- ถอนการติดตั้งแอปพลิเคชัน Teams อีกครั้ง
    - เรียกดูโฟลเดอร์ %appdata%\Microsoft\Teams\ บนคอมพิวเตอร์ของคุณ แล้วลบไฟล์ทั้งหมดในไดเรกทอรีนั้น
    - [ดาวน์โหลดและติดตั้งแอป Teams และ](https://www.microsoft.com/microsoft-teams/download-app)ถ้าเป็นไปได้ ให้ติดตั้ง Teams ในฐานะผู้ดูแลระบบ (คลิกขวาที่ตัวติดตั้ง Teams แล้วเลือก **เรียกใช้** ในฐานะผู้ดูแลระบบ ถ้ามี)

ถ้าไคลเอ็นต์ Teamsของคุณยังคงหยุดการได้รับความเสียหาย ให้ลองให้เกิดปัญหานี้อีกครั้ง ถ้าคุณสามารถ:

1. ใช้ตัวบันทึกขั้นตอนเพื่อบันทึกขั้นตอนของคุณ
    - ปิดแอปพลิเคชันทั้งหมดโดยไม่จําเป็นหรือเป็นความลับ
    - เรียกใช้ตัวบันทึกขั้นตอน และพบปัญหาขณะเข้าสู่ระบบด้วยบัญชีผู้ใช้ที่ได้รับผลกระทบ
    - [รวบรวมบันทึกทีมที่บันทึกขั้นตอน repro ที่บันทึกไว้](https://docs.microsoft.com/microsoftteams/log-files) 
    
    **หมายเหตุ**: ตรวจสอบให้แน่ใจว่าคุณจับภาพที่อยู่การลงชื่อเข้าใช้ของผู้ใช้ที่มีผลกระทบ
    - รวบรวมข้อมูลการเก็บและ/หรือข้อมูลกลุ่มความผิดพลาด (Windows) เรียกใช้Windows Powershell บนคอมพิวเตอร์ที่เกิดการหยุดหยุดและเรียกใช้สั่งต่อไปนี้ (หลังจากแต่ละการสั่ง ให้กด Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. หลังจากไฟล์ข้อความถูกสร้างขึ้นและปรากฏบนหน้าจอของคุณ ให้บันทึกไฟล์และแนบไฟล์ลงในการร้องขอบริการ 
