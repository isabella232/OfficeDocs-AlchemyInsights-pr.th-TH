---
title: ค้นหาและลบข้อความอีเมลในองค์กรของคุณ
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948902"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>ค้นหาและลบข้อความอีเมลในองค์กรของคุณ

ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. ถ้าคุณไม่ได้เป็นผู้ดูแลระบบส่วนกลาง เมื่อต้องการค้นหาข้อความ ในบัญชีผู้ใช้ของคุณต้องถูกเพิ่มลงในกลุ่มบทบาท ตัวจัดการ **eDiscovery** หรือ **บทบาทการจัดการการค้นหาการปฏิบัติตาม** นโยบาย เมื่อต้องการลบข้อความ คุณจะต้องเข้าร่วมกลุ่มบทบาท **การจัดการองค์กร** หรือ **บทบาทการจัดการการค้นหาและล้าง** สิทธิ์ของบทบาทเหล่านี้จะถูกมอบหมายใน [ศูนย์&การปฏิบัติตามนโยบาย](https://protection.office.com)
2. [สร้างการค้นหา](https://docs.microsoft.com/office365/securitycompliance/content-search) เนื้อหาเพื่อค้นหาข้อความที่จะลบ
3. [เชื่อมต่อศูนย์การรักษา&การปฏิบัติตามนโยบายของ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) ถ้าคุณใช้งาน MFA ให้ดูคําแนะนําเหล่านี้: เชื่อมต่อ[ศูนย์&การปฏิบัติตามนโยบายของ PowerShell โดยใช้การรับรองความถูกต้องโดยใช้หลายปัจจัย](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. ลบข้อความ: เรียกใช้ `New-ComplianceSearchAction` cmdlet เพื่อลบข้อความ ข้อความที่ถูกลบจะถูกย้ายไปยังโฟลเดอร์รายการที่กู้คืนได้ของผู้ใช้ ตัวอย่างเช่น การสั่ง ดู [ขั้นตอนที่ 3: ลบข้อความ](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
