---
title: การแก้ไขปัญหาเกี่ยวกับผู้ใช้ที่ไม่รู้จักในการสนทนาทีม
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003807"
- "6809"
ms.openlocfilehash: 523c11cb9d5c4696703c67c2a6b3184f5d12f8e7
ms.sourcegitcommit: d151b09064df3fb573ae07a387a08d98a9553b9b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807776"
---
# <a name="resolving-issue-with-unknown-user-in-teams-chat"></a>การแก้ไขปัญหาเกี่ยวกับ "ผู้ใช้ที่ไม่รู้จัก" ในทีมการแชท

ในบางครั้งผู้ใช้ที่ถูกนำออกจะปรากฏเป็น "ผู้ใช้ที่ไม่รู้จัก" นี่เป็น [ปัญหาที่ทราบ](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown)แล้ว

ถ้าคุณเห็นผู้ใช้ที่แสดงเป็น "ผู้ใช้ที่ไม่รู้จัก" ในการสนทนาทีมให้ลองและล้างแคช:

1.  คลิกขวาที่ไอคอนทีมในแถบงาน คลิก **ออก**
2.  เรียกดูโฟลเดอร์%appdata%\Microsoft\teams\ บนคอมพิวเตอร์ของคุณและลบไฟล์ทั้งหมดในไดเรกทอรีนั้น

คุณสามารถป้องกันไม่ให้ผู้ใช้ที่ไม่ระบุชื่อเข้าร่วมการประชุมได้โดยการตรวจสอบให้แน่ใจว่าพวกเขารออยู่ที่ล็อบบี้ สำหรับข้อมูลเพิ่มเติมให้ดู[ที่เปลี่ยนการตั้งค่าผู้เข้าร่วมสำหรับการประชุมทีม](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e)
