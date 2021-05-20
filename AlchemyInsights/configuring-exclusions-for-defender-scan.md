---
title: การกําหนดค่าข้อยกเว้นMicrosoft Defender ATPสแกน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543704"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a>การกําหนดค่าข้อยกเว้นMicrosoft Defender ATPสแกน

โดยทั่วไปแล้ว คุณสามารถยกเว้นส่วนขยายของไฟล์และโฟลเดอร์บางรายการจากMicrosoft Defender ATPสแกนได้ คุณยังสามารถกําหนดค่าการยกเว้นไฟล์ที่เปิดโดยกระบวนการบางอย่างได้ For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and Configure [exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .

เมื่อต้องการกําหนดค่าการยกเว้น **Windows Server 2016 และ 2019** ให้ดูที่ กําหนดค่าโปรแกรมป้องกันไวรัสของ Microsoft Defender [แยกออกWindowsบนเซิร์ฟเวอร์](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)ของคุณ

**Mac**

For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).

**หมายเหตุ** คุณยังสามารถตรวจสอบรายการยกเว้นโดยใช้ไฟล์ทดสอบ EICAR ได้ For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 

**Linux**

For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).

**หมายเหตุ** คุณยังสามารถตรวจสอบรายการยกเว้นโดยใช้ไฟล์ทดสอบ EICAR ได้ For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 