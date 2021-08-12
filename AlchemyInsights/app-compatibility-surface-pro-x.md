---
title: ความเข้ากันได้ของแอปกับ Microsoft Surface Pro X
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7009"
- "9003951"
ms.openlocfilehash: 8f353d1337415183db1df168406b33594fb5fdb0aac3f13d0afe3e682fa6e3f3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932044"
---
# <a name="app-compatibility-with-microsoft-surface-pro-x"></a>ความเข้ากันได้ของแอปกับ Microsoft Surface Pro X

แอปพลิเคชันจะเรียกใช้แตกต่างกันบนอุปกรณ์เช่น Surface Pro X แอปส่วนใหญ่จะเข้ากันได้ แต่มีข้อจํากัดบางอย่าง ต่อไปนี้คือรายการปัญหาที่คุณอาจพบขณะเรียกใช้แอปพลิเคชัน: 

**โปรแกรมควบคุม** โปรแกรมควบคุมจะได้ผลถ้าได้รับการออกแบบมาWindows 10 ARMบนพีซีแบบพื้นฐาน หากโปรแกรมควบคุมไม่ได้ผล แอปหรือฮาร์ดแวร์ที่โปรแกรมควบคุมนั้นใช้งานไม่ได้ก็จะใช้งานไม่ได้ หากต้องการการสนับสนุนเพิ่มเติมเกี่ยวกับอุปกรณ์ของคุณ โปรดดูWindows 10 ARM[ที่ถามบ่อยเกี่ยวกับพีซี](https://support.microsoft.com/windows/windows-10-arm-based-pcs-faq-477f51df-2e3b-f68f-31b0-06f5e4f8ebb5)หรือตรวจสอบกับผู้ผลิตฮาร์ดแวร์

**แอป 64 บิต (x64)** แอปที่เป็น 64 บิต (x64) จะไม่ใช้งาน คุณจะต้องมีแอป (ARM64) แบบ 64 บิต, แอป 32 บิต (ARM32) หรือแอป 32 บิต (x86) โดยปกติแล้วคุณสามารถค้นหาแอปเวอร์ชัน 32 บิต (x86) ได้ แต่นักพัฒนาแอปบางรายจะมีแอปเพียง 64 บิต (x64) เท่านั้น

**แอปที่ปรับแต่ง** แอปที่ปรับแต่งWindowsการใช้งานของคุณ เช่น เทคโนโลยีช่วยเหลือหรือแอปที่เก็บข้อมูลบนระบบคลาวด์ อาจมีปัญหา หากต้องการเรียนรู้เพิ่มเติม โปรดตรวจสอบกับผู้ผลิตแอปพลิเคชัน

**ซอฟต์แวร์ป้องกันไวรัสของบริษัทอื่น** ซอฟต์แวร์ป้องกันไวรัสของบริษัทอื่นบางตัวไม่สามารถติดตั้งได้ ความปลอดภัยของ Windowsช่วยให้คุณปลอดภัยตลอดอายุการใช้งานที่ได้รับการสนับสนุนของอุปกรณ์ Windows 10ของคุณ

**Windows โทรสารและการสแกน** ตัวเลือกWindows แฟกซ์และการสแกน ไม่พร้อมใช้งานบนWindows 10 ARMที่ใช้พีซีแบบเคลื่อนที่

หากคุณประสบปัญหาในการติดตั้ง ถอนการติดตั้ง หรือติดตั้งแอปใหม่ ให้ดู รายละเอียด [การแก้ไขปัญหา](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-app-install#app-troubleshooting-details)แอป

Except in rare instances, all the keywords should be OR rather than AND.