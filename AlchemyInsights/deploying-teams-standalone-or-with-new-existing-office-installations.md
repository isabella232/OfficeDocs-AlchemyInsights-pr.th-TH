---
title: การปรับใช้Teamsแบบสแตนด์อโลนหรือแบบใหม่หรือที่มีOfficeการติดตั้ง
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102221"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>การปรับใช้Teamsแบบสแตนด์อโลนหรือแบบใหม่หรือที่มีOfficeการติดตั้ง

Microsoft Teamsจะรวมเป็นส่วนหนึ่งของการติดตั้ง ***แบบใหม่Microsoft 365 Apps for enterprise*** Microsoft 365 Apps for business และOffice for Macใหม่ For more information, see [When will Microsoft Teams being included with new installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

นอกจากนี้ ตั้งแต่เวอร์ชัน 1906 ในแชนเนลปัจจุบัน Teams จะถูกเพิ่มลงในการติดตั้ง Microsoft 365 Apps for enterprise (และ Microsoft 365 Apps for business) ที่มีอยู่บนอุปกรณ์ที่ใช้ Windows เมื่อคุณอัปเดตการติดตั้งที่มีอยู่เป็นเวอร์ชันล่าสุด For more information, see [What about existing installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> ถ้าคุณไม่ต้องการรอตามเวลาเปิดให้ใช้งานนี้ คุณสามารถปรับใช้ Teams แบบสแตนด์อโลนให้กับผู้ใช้ของคุณ โดยการปฏิบัติตามคํา[](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)แนะนําเหล่านี้ หรือคุณสามารถให้ผู้ใช้ของคุณติดตั้ง Teams ด้วยตนเอง [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) จาก

ถ้าองค์กรของคุณยังไม่พร้อมที่จะปรับใช้Teams เรามีขั้นตอนที่คุณสามารถปฏิบัติตามเพื่อแยกขั้นตอน ***Teamsการติดตั้งใหม่***[หรือการติดตั้ง](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams)Officeที่มีอยู่ [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) ถ้าคุณต้องการTeams ติดตั้งใหม่ แต่ไม่ต้องการให้ Teams เริ่มโดยอัตโนมัติให้ผู้ใช้หลังจากติดตั้ง ให้ดูที่ ป้องกันไม่ให้[Microsoft Teams เริ่มโดยอัตโนมัติหลังจาก](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)การติดตั้ง

เมื่อต้องการ ***Teams*** ออกจากอุปกรณ์Windowsแอป ให้ดู [ถอนการติดตั้ง Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) To cleanup Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

ถ้าคุณใช้งานคอมพิวเตอร์ที่แชร์ Remote Desktop Services (RDS) หรือ Virtual Desktop Infrastructure (VDI) ให้ดูที่ คอมพิวเตอร์ที่แชร์และสภาพแวดล้อม[VDI Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

หากคุณใช้งาน Office for Mac โปรดดู[Microsoft Teamsบน Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> หลังจากTeamsแล้ว จะได้รับ[การอัปเดตโดยอัตโนมัติทุกๆ](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)สองสัปดาห์ด้วยฟีเจอร์ใหม่และการอัปเดตคุณภาพ 