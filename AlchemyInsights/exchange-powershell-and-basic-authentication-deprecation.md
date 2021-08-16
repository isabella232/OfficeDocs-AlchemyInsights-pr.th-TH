---
title: Exchange การเลิกใช้ PowerShell และการรับรองความถูกต้องพื้นฐาน
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
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069263"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange การเลิกใช้ PowerShell และการรับรองความถูกต้องพื้นฐาน

For the latest information about how to connect to Exchange Online PowerShell without the Basic Authentication, [please go here](https://aka.ms/exops-docs). โมดูล PowerShell V2 ไม่ได้ใช้การรับรองความถูกต้องพื้นฐาน

โปรดทราบว่า การรับรองความถูกต้องพื้นฐานยังคงต้องเปิดใช้งานบนเครื่องไคลเอ็นต์ของคุณ
โมดูล PowerShell V2 ใหม่ใช้การรับรองความถูกต้องแบบใหม่เพื่อสร้างการเชื่อมต่อเพื่อเปิดใช้งาน Cmdlet V2 ที่ใช้ REST ทั้งหมด นอกเหนือจาก cmdlets V2 แล้ว ยังช่วยให้คุณเข้าถึง Cmdlet ของ PowerShell ระยะไกล (RPS) ที่เก่ากว่าซึ่งต้องใช้เซสชัน PowerShell ระยะไกล การสร้างเซสชัน RPS Windowsต้องเปิดใช้งาน WinRM BasicAuth บนเครื่องไคลเอ็นต์แม้ว่าโมดูลจะใช้กลไกการรับรองความถูกต้องแบบใหม่เพื่อรับรองความถูกต้องของบริการ ไปป์ไลน์การรับรองความถูกต้องพื้นฐาน WinRM จะใช้ในการส่งโทเค็นการรับรองความถูกต้องแบบใหม่ ถ้าการรับรองความถูกต้องพื้นฐาน WinRM ถูกปิดใช้งานบนเครื่องไคลเอ็นต์ cmdlets V2 ใหม่จะยังคงสามารถใช้งานต่อไปได้ (แต่ cmdlet RPS ที่เก่ากว่าจะไม่แสดง)
