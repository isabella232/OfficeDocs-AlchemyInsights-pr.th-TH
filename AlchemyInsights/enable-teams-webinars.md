---
title: เปิดใช้งานการสัมมนาTeamsผ่านเว็บ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794037"
---
# <a name="enable-teams-webinars"></a>เปิดใช้งานการสัมมนาTeamsผ่านเว็บ

การสัมมนาผ่านเว็บจะเปิดใช้งานตามค่าเริ่มต้น คุณสามารถจัดการผู้ที่สามารถจัดเวลาและลงทะเบียนการสัมมนาผ่านTeamsผ่านเว็บโดยใช้Teams PowerShell ของคุณ

- ผู้ใช้ทั้งหมดที่สามารถสร้างการประชุมยังสามารถสร้างการประชุมการสัมมนาผ่านเว็บได้ ถ้าคุณต้องการจัดการผู้ที่สามารถจัดเวลาการสัมมนาTeamsผ่านเว็บ *ให้ใช้ AllowMeetingRegistration* 
- ตามค่าเริ่มต้น *WhoCanRegister* จะเปิดใช้งานและ **ตั้งค่าเป็น** ทุกคน ถ้าคุณต้องการปิดการลงทะเบียนการประชุม ให้ตั้งค่า *AllowMeetingRegistration* **เป็น** เท็จ

เมื่อต้องการเปลี่ยนการตั้งค่าเหล่านี้ คุณต้องติดตั้ง[Teams PowerShell](/microsoftteams/teams-powershell-install) นอกจากนี้ นโยบายการประชุมจะถูกบังคับใช้บนTeamsการสัมมนาผ่านเว็บ ตัวอย่างเช่น ถ้าการเข้าร่วมแบบไม่ระบุชื่อถูกปิดใช้งานในการตั้งค่าการประชุม ผู้ใช้ที่ไม่ระบุชื่อไม่สามารถเข้าร่วมการสัมมนาผ่านเว็บได้

เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการกําหนดค่าผู้ที่สามารถลงทะเบียนการสัมมนาผ่านเว็บ [ให้ดู กําหนดค่าผู้ที่สามารถลงทะเบียนการสัมมนาผ่าน](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)เว็บ For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).