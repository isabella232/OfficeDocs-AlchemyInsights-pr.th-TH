---
title: ใช้ PowerShell สําหรับนโยบายและความสัมพันธ์ขององค์กรร่วมกัน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862158"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>ใช้ PowerShell สําหรับนโยบายและความสัมพันธ์ขององค์กรร่วมกัน


สําหรับความสัมพันธ์ขององค์กรโปรดตรวจทานไวยากรณ์และพารามิเตอร์รายละเอียดสําหรับ :[รับสหพันธรัฐ ,](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation)[องค์กรใหม่Relationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set - OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)และลบ - [OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

เมื่อต้องการสร้างนโยบายการแชร์ให้ใช้['ร่วมกันใหม่'](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy) เมื่อต้องการ[ใช้นโยบายการใช้ร่วมกันกับกล่องจดหมายหรือผู้ใช้](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)คุณจําเป็นต้องใช้ชุด[กล่องจดหมาย](https://docs.microsoft.com/powershell/module/exchange/set-mailbox)และ[กล่องจดหมายรับ](https://docs.microsoft.com/powershell/module/exchange/get-mailbox)กับนโยบายที่สร้างขึ้นใหม่ เมื่อต้องการ[ปรับเปลี่ยน ปิดใช้งาน หรือเอานโยบายการใช้ร่วมกัน](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)ออก คุณต้องใช้[การตั้งค่าร่วมกันPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy)และ[เอาใช้งานร่วมกันPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)

**สําหรับความเข้าใจเต็มรูปแบบของหัวข้อนี้โปรดอ่าน :**

[การใช้ร่วมกันในการแลกเปลี่ยนแบบออนไลน์](https://docs.microsoft.com/exchange/sharing/sharing)