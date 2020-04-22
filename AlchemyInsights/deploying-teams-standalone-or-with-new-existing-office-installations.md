---
title: การปรับใช้ Teams เป็นแบบสแตนด์อโลนหรือติดตั้ง Office ใหม่หรือที่มีอยู่
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 4b843407f05db207f3b676c03c7088d3d0ba062e
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704652"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>การปรับใช้ Teams เป็นแบบสแตนด์อโลนหรือติดตั้ง Office ใหม่หรือที่มีอยู่

ขณะนี้ Microsoft Teams ได้รวมเป็นส่วนหนึ่งของ***การติดตั้ง***แอป Microsoft 365 สําหรับธุรกิจองค์กร, Microsoft 365 Apps สําหรับธุรกิจ และ Office for Mac สําหรับข้อมูลเพิ่มเติม ให้ดูที่[Microsoft Teams จะเริ่มต้นมาพร้อมกับการติดตั้ง Office ใหม่เมื่อใด](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

นอกจากนี้ เริ่มต้นด้วยรุ่น 1906 ในสถานีรายเดือน Teams จะถูก***เพิ่มเข้ากับการติดตั้งแอป***Microsoft 365 สําหรับธุรกิจ (และแอป Microsoft 365 สําหรับธุรกิจ) บนอุปกรณ์ที่ใช้ Windows เมื่อคุณปรับปรุงการติดตั้งที่มีอยู่ของคุณให้เป็นรุ่นล่าสุด สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การติดตั้ง Office ที่มีอยู่เป็นอย่างไร](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> ถ้าคุณไม่ต้องการรอกําหนดการ[following these instructions](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)การเปิดตัวนี้

หากองค์กรของคุณไม่พร้อมจะปรับใช้ Teams เรามีขั้นตอนที่คุณสามารถดําเนินการ***เพื่อยกเว้น Teams***จากการติดตั้ง Office[ใหม่](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus)หรือ[ที่มีอยู่](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) ถ้าคุณต้องการให้ Teams ถูกติดตั้ง แต่ไม่ต้องการให้ Teams เริ่มต้นโดยอัตโนมัติสําหรับผู้ใช้หลังจากที่ติดตั้งแล้ว ให้ดูที่[ป้องกันไม่ให้ Microsoft Teams เริ่มทํางานโดยอัตโนมัติหลังจากการติดตั้ง](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

เมื่อต้องการ***ถอนการติดตั้งทีม***จากอุปกรณ์ที่เรียกใช้ Windows ให้ดูที่[การถอนการติดตั้ง Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) เมื่อต้องการล้างข้อมูล Microsoft Teams จากเครื่องเป้าหมายหรือผู้ใช้หลายราย ให้ดูที่[การปรับใช้ Microsoft Teams ล้างข้อมูล](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

ถ้าคุณกําลังใช้คอมพิวเตอร์ที่ใช้ร่วมกัน[Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

ถ้าคุณกําลังใช้ Office สําหรับ Mac ให้ดูที่[การติดตั้ง Microsoft Teams บน Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> หลังจากติดตั้ง Teams แล้ว Teams จะ[อัปเดตโดยอัตโนมัติทุก](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)ๆ สองสัปดาห์ด้วยฟีเจอร์ใหม่และการอัปเดตคุณภาพ 