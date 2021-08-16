---
title: เตรียมการใช้งาน TLS 1.2 ในMicrosoft 365
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
ms.openlocfilehash: 79a9dc3833f8329adeb24d27014d08c14eb93d1f5f840c5cfa2ce10991107b1c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040417"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>เตรียมการใช้งาน TLS 1.2 ในMicrosoft 365

ตั้งแต่วันที่ 31 ตุลาคม 2018 Microsoft 365เปลี่ยนเป็น TLS 1.2 ต่อไป เริ่มตั้งแต่วันที่ 15 ตุลาคม 2020 O365 จะเริ่มการเลิกใช้ TLS 1.0 และ 1.1 ในบริการ Rollout of this change will continue over the next weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020. ตามที่สื่อสารก่อนหน้านี้ (MC126199 ในธ.ค. 2017 MC128929 ในเดือนกุมภาพันธ์ 2018 MC186827 ในเดือนกรกฎาคม 2019 และ MC218794 ในเดือนกรกฎาคม 2020) เราย้ายบริการออนไลน์ของเราทั้งหมดไปยัง Transport Layer Security (TLS) 1.2+ เพื่อให้การเข้ารหัสลับในชั้นเรียนดีที่สุด และเพื่อให้แน่ใจว่าบริการของเรามีความปลอดภัยมากขึ้น ตามค่าเริ่มต้น ลูกค้ายังคงสามารถเลือกให้ TLS 1.0/1.1 บนเซิร์ฟเวอร์และทรัพยากรของพวกเขา แต่ควรสมมติให้มีเพียง TLS 1.2 หรือสูงกว่าเท่านั้นที่จะใช้ได้เมื่อโต้ตอบกับทรัพยากร O365
  
เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการเปลี่ยนแปลงเหล่านี้[โปรดดู](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)[ที่นี่](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)และที่นี่

  