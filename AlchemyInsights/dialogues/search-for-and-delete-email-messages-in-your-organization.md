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
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525444"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>ค้นหาและลบข้อความอีเมลในองค์กรของคุณ

ให้ปฏิบัติตามขั้นตอนเหล่านี้:

1. ถ้าคุณไม่ได้เป็นผู้ดูแลระบบส่วนกลาง เมื่อต้องการค้นหาข้อความที่บัญชีผู้ใช้ของคุณต้องเพิ่มลงในกลุ่มบทบาท **ตัวจัดการ eDiscovery** หรือ **บทบาทการจัดการการค้นหาการปฏิบัติตาม** นโยบาย เมื่อต้องการลบข้อความ คุณจะต้องเข้าร่วมกลุ่มบทบาท **การจัดการองค์กร** หรือบทบาท **การจัดการการค้นหาและล้าง** สิทธิ์ในบทบาทเหล่านี้ได้รับการมอบหมายใน [ศูนย์&การปฏิบัติตามนโยบาย](https://protection.office.com)
2. [สร้างการค้นหา](https://docs.microsoft.com/office365/securitycompliance/content-search) เนื้อหาเพื่อค้นหาข้อความเพื่อลบ
3. [เชื่อมต่อกับศูนย์&การปฏิบัติตามนโยบายของ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) ถ้าคุณใช้งาน MFA ให้ดูคําแนะนําเหล่านี้: เชื่อมต่อกับศูนย์การปฏิบัติตาม [& PowerShell โดยใช้การรับรองความถูกต้องโดยใช้หลายปัจจัย](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. ลบข้อความ: เรียกใช้ `New-ComplianceSearchAction` cmdlet เพื่อลบข้อความ ข้อความที่ถูกลบจะถูกย้ายไปยังโฟลเดอร์รายการที่กู้คืนได้ของผู้ใช้ ตัวอย่างเช่น ดูขั้นตอนที่ [3: ลบข้อความ](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
