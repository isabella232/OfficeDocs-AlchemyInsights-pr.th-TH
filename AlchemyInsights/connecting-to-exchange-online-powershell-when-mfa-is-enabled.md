---
title: Connecting 761 การแลกเปลี่ยน PowerShell ออนไลน์เมื่อมีการเปิดใช้งาน MFA
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 4/26/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 761
ms.assetid: 9b0b89e3-d1d7-4e4d-93de-bb4cd00904d8
ms.openlocfilehash: d9c4195ba3079d35f7a556b91ea6d7318efb35cb
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408199"
---
# <a name="connect-to-exchange-online-powershell-when-mfa-is-enabled"></a>เชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนเมื่อมีการเปิดใช้งาน MFA

ถ้าบัญชีของคุณได้เปิดใช้งานด้วยหลายปัจจัยการตรวจสอบ (MFA) คุณจำเป็นต้องทำตามคำแนะนำเหล่านี้เพื่อเชื่อมต่อกับ PowerShell ออนไลน์ของ Exchange: [PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนการเชื่อมต่อโดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

**หมายเหตุ**: แม้ว่าคุณได้เชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนในอดีตโดยใช้[คำสั่งการเชื่อมต่อทั่วไป](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)คุณต้องใช้คำแนะนำในการเชื่อมต่อ MFA หลังจาก MFA ได้ถูกเปิดใช้งานสำหรับบัญชีผู้ใช้ของคุณ
