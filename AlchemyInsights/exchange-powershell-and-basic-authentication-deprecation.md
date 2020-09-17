---
title: การแผนการรับรองความถูกต้องของ Exchange PowerShell และ basic
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: f4f0f63112d639101ea9e9d7e9a9c16a32de4cf3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782994"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>การแผนการรับรองความถูกต้องของ Exchange PowerShell และ basic

สำหรับข้อมูลล่าสุดเกี่ยวกับวิธีการเชื่อมต่อกับ Exchange Online PowerShell โดยไม่ต้องใช้การรับรองความถูกต้องพื้นฐาน[โปรดไปที่นี่](https://aka.ms/exops-docs) โมดูลของ PowerShell V2 ไม่ใช้การรับรองความถูกต้องพื้นฐาน

โปรดทราบว่าการรับรองความถูกต้องพื้นฐานยังคงจำเป็นต้องเปิดใช้งานบนเครื่องไคลเอ็นต์ของคุณ
โมดูลของ PowerShell V2 ใหม่ใช้การรับรองความถูกต้องสมัยใหม่ในการสร้างการเชื่อมต่อสำหรับการเปิดใช้งาน Cmdlet ของ Cmdlet V2 ทั้งหมด นอกเหนือจาก cmdlet ของ V2 แล้วยังช่วยให้คุณสามารถเข้าถึง Cmdlet ของ PowerShell ระยะไกล (RPS) รุ่นเก่าซึ่งจำเป็นต้องมีเซสชัน PowerShell ระยะไกลที่จะถูกสร้างขึ้น การสร้างเซสชัน RPS บนเครื่อง Windows ต้องการให้ WinRM BasicAuth เปิดใช้งานบนเครื่องไคลเอ็นต์แม้ว่าโมดูลที่ใช้กลไกการรับรองความถูกต้องที่ทันสมัยในการรับรองความถูกต้องของบริการ ขั้นตอนการรับรองความถูกต้องของ WinRM Basic จะใช้สำหรับการขนส่งโทเค็นการรับรองความถูกต้องที่ทันสมัย ถ้ามีการปิดใช้งานการรับรองความถูกต้องของ WinRM Basic บนเครื่องไคลเอ็นต์ cmdlet V2 ใหม่จะยังคงทำงาน (แต่ cmdlet ของ RPS ที่เก่ากว่าจะไม่)
