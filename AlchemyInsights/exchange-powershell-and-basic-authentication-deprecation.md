---
title: การแลกเปลี่ยน PowerShell และการเลิกใช้การรับรองความถูกต้องพื้นฐาน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: a0f01d7ecaa444777aa0675795e588790ab22f19
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/22/2020
ms.locfileid: "45205214"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>การแลกเปลี่ยน PowerShell และการเลิกใช้การรับรองความถูกต้องพื้นฐาน

สําหรับข้อมูลล่าสุดเกี่ยวกับวิธีการเชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนโดยไม่ต้องใช้การรับรองความถูกต้องพื้นฐาน[โปรดไปที่ที่นี่](https://aka.ms/exops-docs) โมดูล PowerShell V2 ไม่ได้ใช้การรับรองความถูกต้องพื้นฐาน

โปรดทราบว่าการรับรองความถูกต้องพื้นฐานยังคงต้องเปิดใช้งานบนเครื่องไคลเอ็นต์ของคุณ
โมดูล PowerShell V2 ใหม่ใช้การรับรองความถูกต้องสมัยใหม่เพื่อสร้างการเชื่อมต่อสําหรับการเปิดใช้งาน Cmdlet ของ V2 ที่ใช้ REST ทั้งหมด นอกจาก cmdlet ของ V2 ก็ยังช่วยให้คุณสามารถเข้าถึง Cmdlet ของ PowerShell ระยะไกล (RPS) เก่าซึ่งต้องใช้เซสชัน PowerShell ระยะไกลที่จะจัดตั้งขึ้น การสร้างเซสชัน RPS บนเครื่อง Windows ต้อง WinRM BasicAuth เพื่อเปิดใช้งานบนเครื่องไคลเอนต์แม้ว่าโมดูลใช้กลไกการรับรองความถูกต้องแบบสมัยใหม่เพื่อรับรองความถูกต้องกับบริการ ขั้นตอนการตรวจสอบพื้นฐาน WinRM ถูกใช้สําหรับการขนส่งโทเค็นการรับรองความถูกต้องสมัยใหม่ ถ้า WinRM พื้นฐานการรับรองความถูกต้องถูกปิดใช้งานบนเครื่องไคลเอ็นต์ cmdlets V2 ใหม่จะยังคงทํางานต่อไป (แต่ cmdlet ของ RPS เก่าจะไม่)
