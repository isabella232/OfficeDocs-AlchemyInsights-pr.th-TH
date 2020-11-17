---
title: เตรียมพร้อมสำหรับการใช้งาน TLS ๑.๒ใน Microsoft ๓๖๕
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085923"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>เตรียมพร้อมสำหรับการใช้งาน TLS ๑.๒ใน Microsoft ๓๖๕

ณวันที่31ตุลาคม๒๐๑๘ Microsoft ๓๖๕จะดำเนินการเปลี่ยนไปยัง TLS ๑.๒ต่อไป เริ่มต้นวันที่15ตุลาคม๒๐๒๐ O365 จะเริ่มต้นแผนของ TLS ๑.๐และ๑.๑บนบริการ ไวร์ของการเปลี่ยนแปลงนี้จะดำเนินการต่อไปอีกไม่กี่สัปดาห์และเดือนแต่ลูกค้าควรสันนิษฐานว่าไม่มี TLS 1.0/1.1 การโทรจะทำงานเมื่อมีส่วนร่วมกับ O365 เริ่มต้นวันที่15ตุลาคม๒๐๒๐ ตามที่สื่อสารก่อนหน้านี้ (MC126199 ใน Dec ๒๐๑๗, MC128929 ใน Feb ๒๐๑๘, MC186827 ในเดือนกรกฎาคม๒๐๑๙และ MC218794 ในเดือนกรกฎาคม๒๐๒๐) เราจะย้ายบริการออนไลน์ทั้งหมดของเราไปยังการขนส่งชั้นความปลอดภัย (TLS) 1.2 + เพื่อให้การเข้ารหัสลับที่ดีที่สุดและเพื่อให้แน่ใจว่าบริการของเรามีความปลอดภัยมากขึ้นตามค่าเริ่มต้น ลูกค้ายังสามารถเลือกที่จะมี TLS 1.0/1.1 บนเซิร์ฟเวอร์และทรัพยากรของพวกเขาแต่ควรจะมีเฉพาะ TLS ๑.๒หรือสูงกว่าจะทำงานเมื่อมีการโต้ตอบกับทรัพยากร O365
  
เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการเปลี่ยนแปลงเหล่านี้โปรดดู[ที่นี่](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)และ[ที่นี่](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)

  