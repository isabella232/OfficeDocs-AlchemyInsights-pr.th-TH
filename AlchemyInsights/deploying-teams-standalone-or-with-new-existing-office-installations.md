---
title: ปรับใช้ทีม เป็นแบบสแตนด์อโลน หรือ ด้วยการติดตั้ง Office ใหม่ หรือที่มีอยู่
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054249"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>ปรับใช้ทีม เป็นแบบสแตนด์อโลน หรือ ด้วยการติดตั้ง Office ใหม่ หรือที่มีอยู่

ทีมงาน Microsoft อยู่ในขณะนี้รวมอยู่เป็นส่วนหนึ่งของการ***ติดตั้งใหม่***ของ Office 365 ProPlus, Office 365 ธุรกิจ และ Office สำหรับ Mac. สำหรับข้อมูลเพิ่มเติม ดู[เมื่อจะทีม Microsoft เริ่มต้นที่มาพร้อมกับการติดตั้ง Office ใหม่หรือไม่?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

นอกจากนี้ เริ่มต้น ด้วยรุ่น 1906 ในช่องรายเดือน ทีมจะ***เพิ่มการติดตั้งที่มีอยู่***ของ Office 365 ProPlus (และ Office 365 ธุรกิจ) บนอุปกรณ์ที่ใช้ Windows เมื่อคุณปรับปรุงการติดตั้งที่มีอยู่เป็นรุ่นล่าสุด สำหรับข้อมูลเพิ่มเติม ดู[อะไรเกี่ยวกับการติดตั้ง Office ที่มีอยู่หรือไม่?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> ถ้าคุณไม่ต้องการรอสำหรับกำหนดการไวร์นี้ คุณสามารถปรับใช้ทีมเป็นแบบสแตนด์อโลนสำหรับผู้ใช้ของคุณโดย[ทำตามคำแนะนำเหล่านี้](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) หรือคุณสามารถให้ผู้ใช้ของคุณติดตั้งทีมงานให้กับพวกเขาเองจาก [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)ได้

ถ้าองค์กรของคุณไม่พร้อมใช้งานในทีม เรามีขั้นตอนคุณสามารถนำไปใช้ในการ***แยกกลุ่มคน***จากการติดตั้ง[ใหม่](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus)หรือ[ที่มีอยู่](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams)ของสำนักงาน ถ้าคุณต้องการให้ทีมสามารถติด ตั้ง แต่ไม่ต้องทีมงานจะเริ่มต้นโดยอัตโนมัติสำหรับผู้ใช้หลังจากที่มีการติดตั้ง ดู[ทีมงาน Microsoft ป้องกันไม่ให้เริ่มทำงานโดยอัตโนมัติหลังจากการติดตั้ง](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

เมื่อต้องการ***ถอนการติดตั้งทีมงาน***จากอุปกรณ์ใช้ Windows ดู[ทีมงานการถอนการติดตั้ง Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) เมื่อต้องการล้างข้อมูลทีม Microsoft จากเครื่องเป้าหมายหรือผู้ใช้หลาย ดู[ล้างข้อมูลการปรับใช้ Microsoft ทีม](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

ถ้าคุณกำลังใช้คอมพิวเตอร์ที่ใช้ร่วมกัน บริการเดสก์ท็อประยะไกล (RDS), หรือโครงสร้างพื้นฐานเดสก์ท็อปเสมือน (VDI), ดู[คอมพิวเตอร์ที่ใช้ร่วมกันและสภาพแวดล้อม VDI กับทีมงานของ Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

ถ้าคุณกำลังใช้ Office สำหรับ Mac ดู[การติดตั้ง Microsoft ทีมบน Mac เป็น](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> หลังจากที่มีการติดตั้ง ทีมงานจะ[อัพเดตโดยอัตโนมัติ](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)โดยประมาณทุกสองสัปดาห์ ด้วยคุณลักษณะใหม่ ๆ และการปรับปรุงคุณภาพ 