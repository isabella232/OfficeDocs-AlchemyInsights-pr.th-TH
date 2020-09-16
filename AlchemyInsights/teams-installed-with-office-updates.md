---
title: ทีมที่ติดตั้งด้วยการอัปเดต Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: 9a09800fcc36876629c7d59182f20b5b16393ef8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47736523"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>ทีม Microsoft ที่ติดตั้งด้วยการอัปเดต Office

ทีม microsoft จะรวมอยู่ในการ ***ติดตั้งใหม่*** ของแอป microsoft ๓๖๕สำหรับองค์กรแอป microsoft ๓๖๕สำหรับธุรกิจและ Office for Mac สำหรับข้อมูลเพิ่มเติมให้ดู [เวลาที่ทีม Microsoft จะเริ่มรวมเข้ากับการติดตั้ง Office ใหม่ใช่หรือไม่](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

นอกจากนี้การเริ่มต้นด้วยเวอร์ชัน๑๙๐๖ในแชนเนลปัจจุบันทีมจะค่อยๆเพิ่มไปยังการ ***ติดตั้ง*** แอป microsoft ๓๖๕สำหรับองค์กร (และแอป microsoft ๓๖๕ for business) บนอุปกรณ์ที่ใช้ Windows เมื่อคุณอัปเดตการติดตั้งที่มีอยู่ของคุณเป็นเวอร์ชันล่าสุด สำหรับข้อมูลเพิ่มเติมให้ดู [ที่อะไรเกี่ยวกับการติดตั้ง Office ที่มีอยู่](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**หมายเหตุ:** ถ้าคุณไม่ต้องการรอสำหรับกำหนดการไวร์นี้คุณสามารถปรับใช้ทีมเป็นแบบสแตนด์อโลนสำหรับผู้ใช้ของคุณได้โดยทำตาม [คำแนะนำเหล่านี้](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)หรือคุณสามารถทำให้ผู้ใช้ของคุณติดตั้งทีมสำหรับตัวเอง https://teams.microsoft.com/downloads ได้

ถ้าองค์กรของคุณไม่พร้อมที่จะปรับใช้ทีมคุณสามารถ ***แยกทีม*** ออกจากการติดตั้ง Office [ใหม่](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) หรือ [ที่มีอยู่](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) แล้วได้ ถ้าคุณต้องการติดตั้งทีมแต่ไม่ต้องการให้ทีมเริ่มต้นโดยอัตโนมัติสำหรับผู้ใช้หลังจากที่ติดตั้งอยู่ให้ดูที่[ป้องกันไม่ให้ทีม Microsoft เริ่มต้นโดยอัตโนมัติหลังจากการติดตั้ง](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

เมื่อต้อง***การถอนการติดตั้งทีม***จากอุปกรณ์ที่ใช้ Windows ให้ดูที่[ถอนการติดตั้งทีม Microsoft](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81) เมื่อต้องการล้างข้อมูลทีม Microsoft จากเครื่องจักรเป้าหมายหรือผู้ใช้หลายคนให้ดูที่การ[ล้างข้อมูลการปรับใช้ของทีม microsoft](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

ถ้าคุณกำลังใช้คอมพิวเตอร์ที่ใช้ร่วมกันบริการเดสก์ท็อประยะไกล (RDS) หรือโครงสร้างพื้นฐานเดสก์ท็อปเสมือน (VDI) ให้ดู[ที่สภาพแวดล้อมของคอมพิวเตอร์ที่แชร์และ VDI กับทีม Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams) ถ้าคุณกำลังใช้ Office for Mac ให้ดูที่[การติดตั้ง Microsoft team บน Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**หมายเหตุ:** หลังจากติดตั้งทีมแล้วจะมีการ [อัปเดตโดยอัตโนมัติ](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) ทุกสองสัปดาห์ด้วยฟีเจอร์และการอัปเดตที่มีคุณภาพใหม่ 