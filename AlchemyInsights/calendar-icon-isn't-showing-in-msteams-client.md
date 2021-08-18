---
title: ไอคอนปฏิทินไม่แสดงในMicrosoft Teamsไคลเอ็นต์
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120023"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>ไอคอนปฏิทินไม่แสดงในMicrosoft Teamsไคลเอ็นต์

แท็บ **ปฏิทิน** ใน Teamsต้องเข้าถึงกล่องจดหมายExchangeผ่านทางExchangeบริการเว็บ กล่องจดหมายExchangeกล่องจดหมายสามารถเป็นออนไลน์หรือภายในองค์กรได้ For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). ถ้าผู้ใช้ของคุณอยู่ในระบบภายในองค์กร คุณต้องยืนยันว่าการกําหนดค่าแบบไฮบริดของคุณสมบูรณ์ ใช้ตัวช่วยสร้าง [การกําหนดค่าแบบ](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) ไฮบริดเพื่อแก้ไขปัญหา โปรดทราบว่า Teams[ต้องใช้Exchange 2016 CU3 หรือสูงกว่า](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)

For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
