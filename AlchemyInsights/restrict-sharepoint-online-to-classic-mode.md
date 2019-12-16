---
title: จำกัด SharePoint แบบออนไลน์ไปยังโหมดคลาสสิก
ms.author: pebaum
author: pebaum
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048779"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>จำกัด SharePoint แบบออนไลน์ไปยังโหมดคลาสสิก

บางองค์กรยังคงต้องการประสบการณ์ใช้งานโหมดคลาสสิก ในขณะที่ไม่มีแผนการลบโหมดคลาสสิกในระดับที่ละเอียดไม่สามารถจำกัดทั้งองค์กร (ผู้เช่า) ไปยังโหมดคลาสสิกสำหรับรายการและไลบรารีได้อีกต่อไป

ผู้ดูแลจะมีตัวเลือกต่อไปนี้ในการจัดการรายการและไลบรารีในโหมดคลาสสิกโดยใช้สวิตช์การเลือกที่เป็นเม็ดที่เราให้ไว้ในระดับต่อไปนี้:

- ชุดเก็บรวบรวมไซต์
- ไซต์
- รายการ
- ไลบ รา รี

นอกจากนี้รายการที่ใช้คุณลักษณะบางอย่างและการกำหนดเองที่ไม่ได้รับการสนับสนุนโดยแบบสมัยใหม่จะยังคงถูกสลับไปยังโหมดคลาสสิกโดยอัตโนมัติ

เริ่มต้นวันที่1เมษายน๒๐๑๙กระบวนการปิดใช้งานระดับผู้เช่าไม่เลือกจากรายการที่ทันสมัยและไลบรารีจะเริ่มต้นและดำเนินการต่อถึง31พฤษภาคม๒๐๑๙  รายการและไลบรารีที่อยู่ในโหมดคลาสสิกเป็นผลมาจากการเลือกไม่ใช้ผู้เช่าจะถูกเลื่อนไปทันสมัยโดยอัตโนมัติ

หากคุณต้องการโหมดคลาสสิกโปรดดูข้อมูลเพิ่มเติมที่[นี่](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)และคำแนะนำของ Powershell PnP ที่[นี่](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout)ซึ่งอธิบายถึงตัวเลือกและเครื่องมือที่คุณสามารถใช้ในวันนี้เพื่อใช้ประสบการณ์ในโหมดคลาสสิก
