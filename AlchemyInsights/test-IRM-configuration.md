---
title: ทดสอบการกําหนดค่า IRM เพื่อความสามารถใหม่ของ OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 22430e2b8a00023f9922fd59d6fcabd308d08453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317251"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>ทดสอบการกําหนดค่า IRM เพื่อความสามารถใหม่ของ OME

เมื่อต้องการตรวจสอบว่าผู้Microsoft 365ของคุณได้รับการกําหนดค่าให้ใช้ความสามารถ OME ใหม่ ให้เรียกใช้ cmdlets ต่อไปนี้ในขณะที่Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell):


1. ตรวจสอบการกําหนดค่า IRM ของผู้เช่าของคุณโดย `Get-IRMConfiguration` การเรียกใช้ ตรวจสอบให้แน่ใจว่าค่าเหล่านี้ถูกตั้งค่าเป็น **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. ใช้โดเมน ที่อยู่ผู้ส่ง และผู้รับ `Test-IRMConfiguration` ของคุณ เรียกใช้ ถ้าการทดสอบไม่ผ่าน ให้ตรวจสอบการกําหนดค่า IRM ของคุณ

For more info about how to verify IRM configuration, see [Verify new OME configuration in Exchange Online PowerShell](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).