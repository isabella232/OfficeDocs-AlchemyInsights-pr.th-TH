---
title: ไอคอนปฏิทินไม่แสดงในไคลเอ็นต์ Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932382"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>ไอคอนปฏิทินไม่แสดงในไคลเอ็นต์ Teams

แท็บปฏิทินในทีมต้องเข้าถึงกล่องจดหมาย Exchange ผ่านทางเว็บเซอร์วิสของอัตราแลกเปลี่ยน กล่องจดหมาย Exchange สามารถออนไลน์หรือในสถาน สําหรับผู้ใช้ออนไลน์ที่ไม่เห็นแท็บปฏิทินตรวจสอบให้แน่ใจว่า[พวกเขาจะได้รับอนุญาตสําหรับกล่องจดหมาย Exchange แบบออนไลน์ และกล่องจดหมายถูกเปิดใช้งาน](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)

ถ้าผู้ใช้มีกล่องจดหมายที่ถูกต้องใน Exchange แบบออนไลน์ แต่ยังคงไม่สามารถเห็นแท็บปฏิทินคุณอาจประสบปัญหาเครือข่าย ใช้[ตัววิเคราะห์การเชื่อมต่อระยะไกลของ Microsoft](https://testconnectivity.microsoft.com/)และเรียกใช้**การทดสอบการเชื่อมต่อบริการเว็บ Exchange Microsoft**สําหรับผู้ใช้ที่ได้รับผลกระทบ

สุดท้ายตรวจสอบ[แอปทีม - นโยบายการตั้งค่าแอป](https://admin.teams.microsoft.com/policies/app-setup)เพื่อให้แน่ใจว่าแอปปฏิทินไม่ได้ถูกลบออกจากนโยบายที่นําไปใช้กับผู้ใช้ (ส่วนใหญ่น่าจะเป็น**แบบส่วนกลาง (ค่าเริ่มต้นทั้งองค์กร)**

หากผู้ใช้ของคุณ homed ในสถานที่ คุณจําเป็นต้องยืนยันว่าการกําหนดค่าไฮบริดของคุณมีสุขภาพดี ใช้[ตัวช่วยสร้างการตั้งค่าคอนฟิกไฮบริดสลี](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)การแก้ไขปัญหา

โปรดทราบว่า[ทีมต้องการ CU3 2016 ของ Exchange หรือสูงกว่า](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)
