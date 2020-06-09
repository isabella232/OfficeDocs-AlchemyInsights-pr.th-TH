---
title: การปรับใช้ Teams เป็นแบบสแตนด์อโลน หรือ กับการติดตั้ง Office ใหม่หรือที่มีอยู่
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
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617914"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>การปรับใช้ Teams เป็นแบบสแตนด์อโลน หรือ กับการติดตั้ง Office ใหม่หรือที่มีอยู่

ขณะนี้ Microsoft Teams จะรวมเป็นส่วนหนึ่งของ***การติดตั้ง***ใหม่ของ Microsoft 365 Apps สําหรับองค์กร Microsoft 365 Apps สําหรับธุรกิจ และ Office สําหรับ Mac สําหรับข้อมูลเพิ่มเติม ให้ดูที่[Microsoft Teams จะเริ่มมาพร้อมกับการติดตั้ง Office ใหม่เมื่อใด](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

นอกจากนี้, เริ่มต้นด้วยรุ่น 1906 ในช่องทางปัจจุบัน, ทีมจะถูก***เพิ่มการติดตั้งที่มีอยู่***ของ Microsoft 365 Apps สําหรับองค์กร (และ Microsoft 365 Apps สําหรับธุรกิจ) บนอุปกรณ์ที่ใช้ Windows เมื่อคุณปรับปรุงการติดตั้งที่มีอยู่ของคุณเป็นรุ่นล่าสุด. สําหรับข้อมูลเพิ่มเติม ให้ดูที่[สิ่งที่เกี่ยวกับการติดตั้ง Office ที่มีอยู่](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> ถ้าคุณไม่ต้องการรอตารางเวลาการเปิดตัวนี้ คุณสามารถปรับใช้ Teams เป็นแบบสแตนด์อโลนสําหรับผู้ใช้ของคุณโดย[ทําตามคําแนะนําเหล่านี้](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   หรือคุณสามารถให้ผู้ใช้ของคุณติดตั้ง Teams ด้วยตนเองจาก  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)

ถ้าองค์กรของคุณยังไม่พร้อมปรับใช้ Teams เรามีขั้นตอนที่คุณสามารถใช้เพื่อ***แยก Teams***ออกจากการติดตั้ง Office[ใหม่](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps)หรือ[ที่มีอยู่](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) ถ้าคุณต้องการให้ทีมได้รับการติดตั้ง แต่ไม่ต้องการให้ทีมเริ่มทํางานโดยอัตโนมัติสําหรับผู้ใช้หลังจากที่มีการติดตั้งแล้ว ให้ดูที่[ป้องกันไม่ให้ทีม Microsoft เริ่มทํางานโดยอัตโนมัติหลังจากการติดตั้ง](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

เมื่อต้องการ***ถอนการติดตั้ง Teams***จากอุปกรณ์ที่ใช้ Windows โปรดดูที่[ถอนการติดตั้ง Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) เมื่อต้องการล้างข้อมูลทีม Microsoft จากเครื่องจักรเป้าหมายหลายเครื่องหรือผู้ใช้ ให้ดูที่[การล้างข้อมูลการปรับใช้ Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

ถ้าคุณกําลังใช้คอมพิวเตอร์ที่ใช้ร่วมกัน[Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

ถ้าคุณกําลังใช้ Office สําหรับ Mac ให้ดูที่[การติดตั้ง Microsoft Teams บน Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> หลังจากติดตั้ง Teams แล้ว ทีมจะ[อัพเดท](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)โดยอัตโนมัติทุกสองสัปดาห์ด้วยคุณสมบัติใหม่และการอัปเดตคุณภาพ 