---
title: การแก้ไขปัญหากับผู้ใช้ที่ไม่รู้จักในTeamsแชท
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
ms.openlocfilehash: 276a073a7213bca4a66dc6b9f27b6c9270a2845c9f2b3aaee791ce28f17e9a75
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109943"
---
# <a name="resolving-issue-with-unknown-user-in-teams-chat"></a>การแก้ไขปัญหาเกี่ยวกับ "ผู้ใช้ที่ไม่รู้จัก" ในการTeamsแชท

ในบางครั้ง ผู้ใช้ที่ถูกเอาออกจะปรากฏเป็น "ผู้ใช้ที่ไม่รู้จัก" นี่เป็น [ปัญหาที่ทราบ](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown)แล้ว

ถ้าคุณเห็นผู้ใช้แสดงเป็น "ผู้ใช้ที่ไม่รู้จัก" ในการสนทนาTeamsอยู่ ให้ลองล้างแคช:

1.  คลิกขวาที่ไอคอนTeamsในแถบงาน คลิกออกจาก
2.  เรียกดูโฟลเดอร์ %appdata%\Microsoft\teams\ บนคอมพิวเตอร์ของคุณ แล้วลบไฟล์ทั้งหมดในไดเรกทอรีนั้น

You can prevent anonymous users from joining meetings by ensuring that they wait in the lobby. For more information, see [Change participant settings for a Teams meeting](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).
