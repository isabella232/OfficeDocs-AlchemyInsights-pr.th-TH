---
title: นโยบายที่ติดตาม
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "3207"
ms.openlocfilehash: 5f7a08f4f4b75612c6d11920d0e7d5cc48f106c695a73d2cf5461af8fa881634
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973818"
---
# <a name="teams-policies"></a>Teamsนโยบาย

Microsoft Teamsการตั้งค่าของคุณจะถูกควบคุมโดยนโยบาย เมื่อต้องการเปลี่ยนแปลง คุณต้องกําหนดค่านโยบายที่เหมาะสม แล้วปรับใช้นโยบายนั้นกับผู้ใช้ วิธีที่รวดเร็วที่สุดในการสิ่งนี้กับผู้ใช้ของคุณทั้งหมดคือการปรับเปลี่ยนนโยบายเริ่มต้นที่ชื่อว่า ส่วนกลาง 

**NOTE** การเปลี่ยนแปลงนโยบาย **_จะใช้เวลาอย่างน้อย 4 ถึง 48 ชั่วโมงเพื่อให้_** มีผล ถ้าคุณสร้างนโยบายแบบปรับแต่งเอง คุณต้องรออย่างน้อย 4 ชั่วโมงก่อนที่คุณจะสามารถเปลี่ยนแปลงเพิ่มเติมได้ จากนั้นคุณสามารถปรับใช้นโยบายนั้นกับผู้ใช้ได้ ซึ่งหมายความว่านโยบายแบบปรับแต่งเองอาจใช้เวลาถึง 48 ชั่วโมงเพื่อให้มีผล นโยบายส่วนกลางจะถูกตั้งเป็นค่าเริ่มต้นของผู้ใช้ทั้งหมด และการเปลี่ยนแปลงนโยบายส่วนกลางอาจใช้เวลาถึง 24 ชั่วโมงเพื่อให้มีผล ถ้าคุณได้สร้างนโยบายแบบปรับแต่งเอง ให้ปรับใช้นโยบายนั้นกับผู้ใช้ และนโยบายดังกล่าวยังไม่มีผลหลังจาก 48 ชั่วโมง หรือคุณได้ปรับเปลี่ยนนโยบายส่วนกลางและรออย่างน้อย 24 ชั่วโมง โปรดเปิดกรณีสนับสนุน

Teamsนโยบายจะถูกแบ่งออกเป็นส่วนต่อไปนี้:

- [Teamsควบคุม](https://docs.microsoft.com/MicrosoftTeams/teams-policies)การค้นหาทีมส่วนตัวของผู้ใช้ในการค้นหาและการสร้างแชนเนลส่วนบุคคล  
- [นโยบายการประชุม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)จะควบคุมสิ่งที่ผู้ใช้สามารถTeamsการประชุมรวมถึงการควบคุมล็อบบี้ For help with lobby issues, like configuring Teams to admit everyone, see [Control lobby settings and levels of participation](https://docs.microsoft.com/alchemyinsights/bypass-lobby).
- [นโยบายการส่งข้อความ](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) จะควบคุมสิ่งที่ผู้ใช้สามารถปฏิบัติได้ด้วยการแชทและข้อความ รวมถึงการเปิดหรือปิดการแชท การลบการแชท การร้องขอการตอบรับการอ่าน การใช้ giphys และสติกเกอร์ และอื่นๆ
- [นโยบายการตั้งค่าแอป](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies) จะควบคุมว่าแอปใดจะพร้อมใช้งานต่อผู้ใช้ รวมถึงแอปที่ปรับแต่งเองและแอปของบริษัทอื่น และลาบากที่แอปปรากฏ  
- นโยบายการเก็บ[ข้อมูล](https://docs.microsoft.com/microsoftteams/retention-policies)Teamsข้อมูลจะพบMicrosoft 365ศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย
- Teamsนโยบายสมุดรายชื่อจะถูกตั้งค่าผ่าน[การค้นหาไดเรกทอรีที่จัดขอบเขต](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search)