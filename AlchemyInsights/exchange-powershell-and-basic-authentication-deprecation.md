---
title: การแลกเปลี่ยน PowerShell และการตรวจสอบพิสูจน์ตัวจริงพื้นฐาน
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
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/13/2020
ms.locfileid: "44015708"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>การแลกเปลี่ยน PowerShell และการตรวจสอบพิสูจน์ตัวจริงพื้นฐาน

สําหรับข้อมูลล่าสุดเกี่ยวกับวิธีการเชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนโดยไม่ต้องใช้การรับรองความถูกต้องพื้นฐาน[โปรดไปที่ที่นี่](https://aka.ms/psbasicauth)

โปรดทราบว่าการตรวจสอบความถูกต้องเบื้องต้นยังคงต้องเปิดใช้งานบนเครื่องไคลเอ็นต์ของคุณ
โมดูล PowerShell V2 ใหม่ใช้การรับรองความถูกต้องสมัยใหม่เพื่อสร้างการเชื่อมต่อสําหรับการเปิดใช้งาน REST-based V2 Cmdlet ทั้งหมด นอกเหนือจาก V2 cmdlets แล้ว ยังช่วยให้คุณเข้าถึง Cmdlets Remote PowerShell (RPS) ที่ต้องใช้เซสชัน PowerShell ระยะไกลเพื่อที่จะสร้าง สร้างเซสชัน RPS บนเครื่อง Windows ต้องใช้ WinRM BasicAuth เมื่อต้องการเปิดใช้งานบนเครื่องไคลเอนต์แม้ว่าโมดูลใช้กลไกการรับรองความถูกต้องสมัยใหม่เพื่อรับรองความถูกต้องกับบริการ ขั้นตอนของ WinRM พื้นฐานการรับรองความถูกต้องถูกใช้สําหรับการขนส่งโทเค็นการรับรองความถูกต้องสมัยใหม่ ถ้า WinRM Basic รับรองความถูกต้องถูกปิดใช้งานบนเครื่องไคลเอนต์ cmdlet V2 ใหม่จะทํางานต่อไป (แต่ cmdlets RPS เก่าจะไม่)
