---
title: ไอคอนปฏิทินไม่แสดงในTeamsไคลเอ็นต์
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
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989610"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>ไอคอนปฏิทินไม่แสดงในTeamsไคลเอ็นต์

แท็บ ปฏิทิน ใน Teamsต้องเข้าถึงกล่องจดหมายExchangeผ่านทางExchangeบริการเว็บ กล่องจดหมายExchangeสามารถเป็นออนไลน์หรือภายในองค์กรได้ For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

ถ้าผู้ใช้มีกล่องจดหมายExchange Online แต่ยังคงไม่เห็นแท็บ ปฏิทิน คุณอาจพบปัญหาเครือข่าย ใช้ [ตัววิเคราะห์การเชื่อมต่อระยะไกลของ](https://testconnectivity.microsoft.com/)ไมโครซอฟท์ และเรียกใช้ **การทดสอบการเชื่อมต่อบริการExchangeของไมโครซอฟท์** ให้กับผู้ใช้ที่ถูกกระทบ

สุดท้าย ให้ตรวจสอบแอป [Teams –](https://admin.teams.microsoft.com/policies/app-setup)นโยบายการตั้งค่าแอปเพื่อให้แน่ใจว่าแอปปฏิทินยังไม่ได้ถูกเอาออกจากนโยบายที่ปรับใช้กับผู้ใช้ (ส่วนใหญ่เป็นนโยบายส่วนกลาง (ค่าเริ่มต้นทั่วทั้งองค์กร **)**

ถ้าผู้ใช้ของคุณอยู่ในระบบภายในองค์กร คุณต้องยืนยันว่าการกําหนดค่าแบบไฮบริดของคุณสมบูรณ์ ใช้ตัวช่วยสร้าง [การกําหนดค่าแบบ](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) ไฮบริดเพื่อแก้ไขปัญหา

โปรดทราบว่า Teams[ต้องใช้Exchange 2016 CU3 หรือสูงกว่า](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)
