---
title: ปัญหาเกี่ยวกับการปลอมแปลง ฟิชชิ่ง หรือการปลอมตัว
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1755
ms.assetid: ''
ms.openlocfilehash: fb10c486833cfb0a1726dce69bc2176b39565e9d
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510051"
---
# <a name="issues-with-spoofing-phishing-or-impersonation"></a>ปัญหาเกี่ยวกับการปลอมแปลง ฟิชชิ่ง หรือการปลอมตัว

เรียนรู้วิธีที่ Microsoft ปกป้องคุณจาก:

- [การปลอมแปลง](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spoofing-protection)

- [ฟิชชิงและการปลอมตัว](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-anti-phishing)

คําแนะนําเพิ่มเติม:

- สําหรับผู้ส่งปลอมที่ดูเหมือนจะมาจากโดเมนของคุณเอง[SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)และ[DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)สามารถช่วยได้

- ตรวจสอบว่าผู้ส่งในโดเมนของคุณไม่ได้ถูกกําหนดค่าให้ข้ามการกรองสแปมโดยใช้กฎการไหลของจดหมาย (หรือที่เรียกว่ากฎการขนส่ง) หรืออนุญาตรายการ สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ข้อควรระวังในการข้ามตัวกรองสแปมของ Microsoft](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters)

- ตรวจสอบว่าผู้ใช้ไม่ได้กําหนดค่ารายการ[รายชื่อผู้ส่งที่ปลอดภัย](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE)ซึ่งอาจอนุญาตให้มีการโจมตีแบบฟิชชิ่งได้

- ลองส่งสแปมและข้อความฟิชชิงที่มีความเชื่อมั่นสูงเพื่อกักกันแทนที่จะใช้โฟลเดอร์อีเมลขยะ สําหรับข้อมูลเพิ่มเติม ให้ดูที่[กักกันข้อความอีเมล](https://docs.microsoft.com/microsoft-365/security/office-365-security/quarantine-email-messages)

**[การรายงานข้อความไปยัง Microsoft](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)คือวิธีที่ดีที่สุดในการแจ้งให้เราทราบว่าตัวกรองมีประสิทธิภาพเพียงใด**
