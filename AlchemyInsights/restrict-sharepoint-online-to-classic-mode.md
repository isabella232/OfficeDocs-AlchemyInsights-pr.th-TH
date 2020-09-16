---
title: จำกัด SharePoint Online เป็นโหมดคลาสสิก
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751442"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>จำกัด SharePoint Online เป็นโหมดคลาสสิก

บางองค์กรยังจำเป็นต้องใช้ประสบการณ์การใช้งานโหมดคลาสสิก ในขณะที่ไม่มีแผนที่จะเอาโหมดคลาสสิกออกจากระดับที่เป็นเม็ดจะไม่สามารถจำกัดทั้งองค์กร (ผู้เช่า) เป็นโหมดคลาสสิกสำหรับรายการและไลบรารีได้อีกต่อไป

ผู้ดูแลระบบจะมีตัวเลือกต่อไปนี้ในการจัดการรายการและไลบรารีแต่ละรายการในโหมดคลาสสิกโดยใช้การสลับการเลือกแบบเม็ดที่เรามีให้ในระดับต่อไปนี้:

- ไซต์คอลเลกชัน
- ไซต์
- รายการ
- ไลบ

นอกจากนี้รายการที่ใช้บางฟีเจอร์และการกำหนดเองที่ไม่ได้รับการสนับสนุนโดยสมัยใหม่จะยังคงถูกสลับไปยังโหมดคลาสสิกโดยอัตโนมัติ

เริ่มต้นวันที่1เมษายน๒๐๑๙กระบวนการปิดใช้งานระดับผู้เช่าเลือกไม่อยู่ในรายการและไลบรารีที่ทันสมัยจะเริ่มต้นและดำเนินการต่อไปจนถึง31พฤษภาคม๒๐๑๙  รายการและไลบรารีที่อยู่ในโหมดคลาสสิกอันเป็นผลมาจากการปฏิเสธการเข้าร่วมของผู้เช่าจะถูกเลื่อนไปยังสมัยใหม่โดยอัตโนมัติ

ถ้าคุณจำเป็นต้องใช้โหมดคลาสสิกโปรดดูข้อมูลเพิ่มเติมที่ [นี่](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) และคำแนะนำในการใช้งาน PnP Powershell ที่ [นี่](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) ซึ่งจะอธิบายตัวเลือกและเครื่องมือที่คุณสามารถใช้ได้ในวันนี้เพื่อใช้ประสบการณ์การใช้งานโหมดคลาสสิก
