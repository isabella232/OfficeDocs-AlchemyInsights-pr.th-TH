---
title: บล็อกผู้ใช้จากการบันทึกการประชุม
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 7eb3fd34ec6f1a2d431ed276b00dd46b5ec6aa73d69b37ef88b1ba0ca6f5d077
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019203"
---
# <a name="block-user-from-recording-meetings"></a>บล็อกผู้ใช้จากการบันทึกการประชุม

ถ้าคุณต้องการป้องกัน **หรือบล็อกผู้ใช้** ที่ระบุไม่ให้บันทึกTeamsการประชุม คุณสามารถบันทึกผ่านการตั้งค่านโยบายTeamsการประชุมได้ In the Microsoft Teams admin center, turn off the **Allow cloud recording setting** in the meeting policy assigned to that user. เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)

เมื่อต้องการตรวจสอบว่าผู้ใช้ที่ระบุได้รับอนุญาตหรือไม่บันทึกการประชุมTeams ให้ใช้การวินิจฉัยการสนับสนุน เรียกใช้คิวรีการสนับสนุนใหม่และพิมพ์ใน **Diag: การบันทึก** การประชุม - การวินิจฉัยจะตรวจสอบการตั้งค่านโยบายของผู้ใช้ที่ระบุและระบุการตั้งค่านโยบายของผู้ใช้ โปรดทราบว่า อาจต้องใช้เวลาสองสามชั่วโมงเพื่อให้การตั้งค่านโยบายใหม่มีผล ดังนั้นถ้าคุณเพิ่งเปลี่ยนแปลง ให้รอสองสามชั่วโมงก่อนที่จะเรียกใช้การวินิจฉัยอีกครั้ง

หากต้องการข้อมูลเพิ่มเติม ให้[ตรวจดู เปิดหรือปิดการบันทึกระบบคลาวด์](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)
