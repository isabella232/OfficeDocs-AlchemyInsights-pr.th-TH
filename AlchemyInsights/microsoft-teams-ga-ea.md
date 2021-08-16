---
title: Microsoft Teams - การเข้าถึงของแขก
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: 2c78fec14d43c5cbf6aebbc889d606eb2f6c4c64af85997f523d06872c911a0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012327"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams - การเข้าถึงของแขก

ถ้าคุณต้องการความช่วยเหลือในการติดต่อสื่อสารกับผู้ใช้ภายนอกองค์กรของคุณใน Teams คุณ need to decider to use [Guest Access or External Access (Federation)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access), or you can use both.

อย่าลืมตรวจสอบ [ความแตกต่างเพื่อเข้าใจ](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) ฟีเจอร์ที่พร้อมใช้งานในแต่ละฟีเจอร์  ตัวอย่างเช่น การเข้าถึงจากภายนอก (การติดต่อกับภายนอก) อนุญาตการสื่อสารแบบ 1:1 เช่น การสนทนาและการแสดงตน  ผู้ใช้ภายนอกไม่สามารถเข้าร่วมในการTeamsร่วมกันได้อย่างไรก็ตาม  ถ้าคุณต้องการให้ผู้ใช้ภายนอกเข้าร่วมและเข้าร่วมในการสนทนาแชนTeamsเนลของคุณ หรือ แชร์ไฟล์ คุณจะต้องเปิด การเข้าถึงแบบ Guest

**ตัวเลือกที่ 1: เปิดใช้งานการเข้าถึงของแขก** ในศูนย์Teamsการจัดการ ให้ไปที่ [Org Wide การตั้งค่า > Guest Access](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration)และเปิด "อนุญาตการเข้าถึงของแขกTeams"  For a tenant with all other default settings, this should be all you need to do.  เมื่อต้องการกําหนดค่าการเข้าถึงของ Guest เอง ตรวจสอบให้แน่ใจว่าคุณได้ปฏิบัติตามขั้นตอนทั้งหมดใน [รายการตรวจสอบการเข้าถึงของ](https://docs.microsoft.com/microsoftteams/guest-access-checklist)แขก เมื่อเสร็จสิ้นสมบูรณ์แล้ว คุณจะต้องรอ [ถึง 24](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) ชั่วโมงเพื่อให้การตั้งค่ามีผล

ถ้าคุณมั่นใจว่าคุณได้เสร็จสิ้นขั้นตอนทั้งหมดในรายการตรวจสอบและมากกว่า 24 ชั่วโมงแล้ว ให้เดินหน้าและลองเพิ่ม ผู้ใช้รับเชิญ [ในทีม](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop)ของคุณ

หากต้องการข้อมูลเพิ่มเติม รวมถึงวิดีโอวิธีใช้ ให้ดูที่ การเข้าถึง[จากผู้ใช้Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)ใน

**ตัวเลือกที่ 2: เปิดใช้งานการเข้าถึงภายนอก (การติดต่อกับภายนอก)** ถ้าคุณต้องการเปิดการเข้าถึงภายนอก (การติดต่อกับภายนอก) ในศูนย์การจัดการ Teams ให้ไปที่การเข้าถึงภายนอก [ของ การตั้งค่า >](https://admin.teams.microsoft.com/company-wide-settings/external-communications)ทั่วทั้งองค์กร และเปิด "ผู้ใช้สามารถสื่อสารกับผู้ใช้ Skype for Business และ Teams ได้" แล้วปฏิบัติตามขั้นตอนทั้งหมดใน อนุญาตให้ผู้ใช้ [Teams](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization)ของคุณแชทและสื่อสารกับผู้ใช้ในองค์กรอื่น
