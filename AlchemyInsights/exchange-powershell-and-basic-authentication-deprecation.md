---
title: การเลิกใช้ Exchange PowerShell และการรับรองความถูกต้องพื้นฐาน
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
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813491"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>การเลิกใช้ Exchange PowerShell และการรับรองความถูกต้องพื้นฐาน

For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs). โมดูล PowerShell V2 ไม่ได้ใช้การรับรองความถูกต้องพื้นฐาน

โปรดทราบว่า การรับรองความถูกต้องพื้นฐานยังคงต้องเปิดใช้งานบนเครื่องไคลเอ็นต์ของคุณ
โมดูล PowerShell V2 ใหม่ใช้การรับรองความถูกต้องแบบใหม่เพื่อสร้างการเชื่อมต่อเพื่อเปิดใช้งาน Cmdlet V2 ที่ใช้ REST ทั้งหมด นอกเหนือจาก cmdlets V2 แล้ว ยังช่วยให้คุณเข้าถึง Cmdlet ของ PowerShell ระยะไกล (RPS) ที่เก่ากว่าซึ่งต้องใช้เซสชัน PowerShell ระยะไกล การสร้างเซสชัน RPS บนเครื่อง Windows ต้องใช้ WinRM BasicAuth เพื่อเปิดใช้งานบนเครื่องไคลเอ็นต์แม้ว่าโมดูลจะใช้กลไกการรับรองความถูกต้องแบบใหม่เพื่อรับรองความถูกต้องของบริการ ไปป์ไลน์การรับรองความถูกต้องพื้นฐาน WinRM จะใช้ในการส่งโทเค็นการรับรองความถูกต้องแบบใหม่ ถ้าการรับรองความถูกต้องพื้นฐาน WinRM ถูกปิดใช้งานบนเครื่องไคลเอ็นต์ cmdlets V2 ใหม่จะยังคงสามารถใช้งานต่อไปได้ (แต่ cmdlet RPS ที่เก่ากว่าจะไม่แสดง)
