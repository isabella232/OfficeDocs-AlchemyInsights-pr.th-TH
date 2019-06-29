---
title: จำกัดการ SharePoint แบบออนไลน์สำหรับโหมดคลาสสิก
ms.author: kirks
author: Techwriter40
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
ms.openlocfilehash: 52c63d8909796f8d0d114a46c5255e4073e8c47d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369792"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>จำกัดการ SharePoint แบบออนไลน์สำหรับโหมดคลาสสิก

ยังคงบางองค์กรจำเป็นต้องมีประสบการณ์การใช้งานโหมดคลาสสิก ในขณะที่ไม่มีแผนการเอาโหมดคลาสสิกที่ระดับ granular จะไม่สามารถจำกัดทั้งองค์กร (ผู้เช่า) ถึงโหมดคลาสสิกสำหรับรายการและไลบรารี

ผู้ดูแลจะมีตัวเลือกต่อไปนี้ในการจัดการแต่ละรายการและไลบรารีในโหมดคลาสสิกใช้สวิตช์เลือกเอาท์ granular ที่เราให้ในระดับดังต่อไปนี้:

- ไซต์คอลเลกชัน
- ไซต์
- รายการ
- ไลบรารี

นอกจากนี้ รายการที่ใช้คุณลักษณะบางอย่างและการกำหนดเองที่ไม่ได้รับการสนับสนุน โดยแบบสมัยใหม่จะยังคงสามารถจะสลับไปยังโหมดคลาสสิก

เริ่มต้นเดือน 1 เมษายน 2019 กระบวนการปิดการใช้งานระดับผู้เช่าเลือกออกจากรายการสมัยใหม่ และไลบรารีจะเริ่มการทำงาน และดำเนินต่อผ่าน 31 พฤษภาคม 2019  รายการและไลบรารีที่อยู่ในโหมดคลาสสิกที่เป็นผลมาจากผู้เช่าเข้าร่วมออก จะโดยอัตโนมัติเลื่อนขึ้นไปสมัยใหม่

หากคุณต้องใช้โหมดคลาสสิกโปรดดูข้อมูลเพิ่มเติม[ที่นี่](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)และคำสั่ง PnP Powershell[ที่นี่](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout)ซึ่งอธิบายถึงตัวเลือกและเครื่องมือที่คุณสามารถใช้วันนี้เพื่อใช้กับประสบการณ์ใช้งานโหมดคลาสสิก
