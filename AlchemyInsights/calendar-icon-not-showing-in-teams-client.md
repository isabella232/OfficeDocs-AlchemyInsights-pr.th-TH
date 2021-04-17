---
title: ไอคอนปฏิทินไม่แสดงในไคลเอ็นต์ Teams
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
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819972"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>ไอคอนปฏิทินไม่แสดงในไคลเอ็นต์ Teams

แท็บ ปฏิทิน ใน Teams ต้องมีสิทธิ์เข้าถึงกล่องจดหมาย Exchange ผ่านทาง Exchange Web Services กล่องจดหมาย Exchange สามารถเป็นแบบออนไลน์หรือภายในองค์กรได้ For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

ถ้าผู้ใช้มีกล่องจดหมายที่ถูกต้องใน Exchange Online แต่ยังคงไม่เห็นแท็บ ปฏิทิน คุณอาจประสบปัญหาเกี่ยวกับเครือข่าย ใช้ [ตัววิเคราะห์การเชื่อมต่อระยะไกลของ](https://testconnectivity.microsoft.com/) ไมโครซอฟท์ และเรียกใช้ **การทดสอบการเชื่อมต่อบริการเว็บ Microsoft Exchange** ให้กับผู้ใช้ได้รับผลกระทบ

สุดท้าย ตรวจสอบแอป [Teams –](https://admin.teams.microsoft.com/policies/app-setup)นโยบายการตั้งค่าแอปเพื่อให้แน่ใจว่าแอปปฏิทินยังไม่ได้ถูกลบออกจากนโยบายที่ปรับใช้กับผู้ใช้ (ส่วนใหญ่คือส่วนกลาง **(ค่าเริ่มต้นทั่วทั้งองค์กร)**

ถ้าผู้ใช้ของคุณอยู่ในระบบภายในองค์กร คุณต้องยืนยันว่าการกําหนดค่าแบบไฮบริดของคุณสมบูรณ์ ใช้ตัวช่วยสร้าง [การกําหนดค่าแบบ](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) ไฮบริดเพื่อแก้ไขปัญหา

โปรดทราบว่า[Teams ต้องใช้ Exchange 2016 CU3 หรือสูงกว่า](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)
