---
title: Connecting 761 การแลกเปลี่ยน PowerShell ออนไลน์เมื่อมีการเปิดใช้งาน MFA
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 4/26/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "761"
- "3500011"
ms.assetid: 9b0b89e3-d1d7-4e4d-93de-bb4cd00904d8
ms.openlocfilehash: 16137ae4f0324ca508676a7ba351e5f97e7125a1
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364536"
---
# <a name="connect-to-exchange-online-powershell-when-mfa-is-enabled"></a>เชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนเมื่อมีการเปิดใช้งาน MFA

ถ้าบัญชีของคุณได้เปิดใช้งานด้วยหลายปัจจัยการตรวจสอบ (MFA) คุณจำเป็นต้องทำตามคำแนะนำเหล่านี้เพื่อเชื่อมต่อกับ PowerShell ออนไลน์ของ Exchange: [PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนการเชื่อมต่อโดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

**หมายเหตุ**: แม้ว่าคุณได้เชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนในอดีตโดยใช้[คำสั่งการเชื่อมต่อทั่วไป](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)คุณต้องใช้คำแนะนำในการเชื่อมต่อ MFA หลังจาก MFA ได้ถูกเปิดใช้งานสำหรับบัญชีผู้ใช้ของคุณ
