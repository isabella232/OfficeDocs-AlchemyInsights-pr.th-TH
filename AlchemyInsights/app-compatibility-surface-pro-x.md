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
ms.openlocfilehash: 085815982a3948a7853326541101d2ed21c1869e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837605"
---
# <a name="app-compatibility-with-microsoft-surface-pro-x"></a>ความเข้ากันได้ของแอปกับ Microsoft Surface Pro X

แอปพลิเคชันจะเรียกใช้บนอุปกรณ์ต่าง ๆ เช่น Surface Pro X แอปส่วนใหญ่จะเข้ากันได้ แต่มีข้อจํากัดบางอย่าง ต่อไปนี้คือรายการปัญหาที่คุณอาจพบขณะเรียกใช้แอปพลิเคชัน: 

**โปรแกรมควบคุม** โปรแกรมควบคุมจะได้ผลถ้าโปรแกรมควบคุมถูกออกแบบมาให้ใช้งานบนพีซีที่ใช้ windows 10 ARMได้ หากโปรแกรมควบคุมไม่ได้ผล แอปหรือฮาร์ดแวร์ที่โปรแกรมควบคุมนั้นใช้งานไม่ได้ก็จะใช้งานไม่ได้ ดูการสนับสนุนเพิ่มเติมเกี่ยวกับอุปกรณ์ของคุณได้ที่ ถามบ่อย [เกี่ยวกับพีซีที่ใช้ windows 10](https://support.microsoft.com/windows/windows-10-arm-based-pcs-faq-477f51df-2e3b-f68f-31b0-06f5e4f8ebb5) ARM หรือตรวจสอบกับผู้ผลิตฮาร์ดแวร์

**แอป 64 บิต (x64)** แอปที่เป็น 64 บิต (x64) จะไม่ใช้งาน คุณจะต้องมีแอป (ARM64) แบบ 64 บิต, แอป 32 บิต (ARM32) หรือแอป 32 บิต (x86) โดยปกติแล้วคุณสามารถค้นหาแอปเวอร์ชัน 32 บิต (x86) ได้ แต่นักพัฒนาแอปบางรายจะมีแอปเพียง 64 บิต (x64) เท่านั้น

**แอปที่ปรับแต่ง** แอปที่ปรับแต่งประสบการณ์การใช้งาน Windows เช่น เทคโนโลยีช่วยเหลือหรือแอปที่เก็บข้อมูลบนระบบคลาวด์ อาจมีปัญหา หากต้องการเรียนรู้เพิ่มเติม โปรดตรวจสอบกับผู้ผลิตแอปพลิเคชัน

**ซอฟต์แวร์ป้องกันไวรัสของบริษัทอื่น** ซอฟต์แวร์ป้องกันไวรัสของบริษัทอื่นบางตัวไม่สามารถติดตั้งได้ ความปลอดภัยของ Windows ช่วยรักษาความปลอดภัยให้คุณได้รับการสนับสนุนตลอดอายุการใช้งานอุปกรณ์ Windows 10 ของคุณ

**โทรสารและการสแกนของ Windows** โทรสารและการสแกนของ Windows ไม่พร้อมใช้งานบนพีซีที่ใช้ windows 10 ARMอื่น

หากคุณประสบปัญหาในการติดตั้ง ถอนการติดตั้ง หรือติดตั้งแอปใหม่ ให้ดู รายละเอียด [การแก้ไขปัญหา](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-app-install#app-troubleshooting-details)แอป

Except in rare instances, all the keywords should be OR rather than AND.