---
title: ไอคอนปฏิทินที่ไม่แสดงในไคลเอ็นต์ของทีม
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
- "9001219"
- "4375"
ms.openlocfilehash: f30cd5bda62756cf6b912ed150b4e59e7ca4d85d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684717"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>ไอคอนปฏิทินที่ไม่แสดงในไคลเอ็นต์ของทีม

แท็บปฏิทินในทีมจำเป็นต้องมีสิทธิ์การเข้าถึงกล่องจดหมาย Exchange ผ่านทางเว็บเซอร์วิส Exchange กล่องจดหมาย Exchange สามารถออนไลน์หรือภายในองค์กรได้ สำหรับผู้ใช้ออนไลน์ที่ไม่เห็นแท็บปฏิทินตรวจสอบให้แน่ใจว่า[ได้รับสิทธิ์การใช้งานสำหรับกล่องจดหมาย Exchange Online และกล่องจดหมายถูกเปิดใช้งาน](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)

ถ้าผู้ใช้มีกล่องจดหมายที่ถูกต้องใน Exchange Online แต่ยังไม่สามารถเห็นแท็บปฏิทินคุณอาจพบปัญหาเครือข่าย ใช้ตัว [วิเคราะห์การเชื่อมต่อระยะไกลของ microsoft](https://testconnectivity.microsoft.com/) และเรียกใช้การ **ทดสอบการเชื่อมต่อบริการเว็บ microsoft Exchange** สำหรับผู้ใช้ที่ได้รับผลกระทบ

ในที่สุดการตรวจสอบ[แอปทีม–นโยบายการตั้งค่าแอป](https://admin.teams.microsoft.com/policies/app-setup)เพื่อให้แน่ใจว่าแอปปฏิทินไม่ได้ถูกเอาออกจากนโยบายที่ถูกนำไปใช้กับผู้ใช้ (ที่เป็นไปได้มากที่สุดคือส่วน**กลาง (ค่าเริ่มต้นทั้งองค์กร)**

ถ้าผู้ใช้ของคุณได้รับการ homed ภายในองค์กรคุณจำเป็นต้องยืนยันการกำหนดค่าไฮบริดของคุณที่มีสุขภาพดี ใช้ [ตัวช่วยสร้างการกำหนดค่าแบบไฮบริดเพื่อ](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) แก้ไขปัญหา

โปรดทราบว่า[ทีมจำเป็นต้องมี Exchange ๒๐๑๖ CU3 หรือสูงกว่า](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)
