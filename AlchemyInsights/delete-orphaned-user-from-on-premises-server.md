---
title: ลบผู้ใช้ที่ถูกไม่มีสิทธิ์ออกจากเซิร์ฟเวอร์ภายในองค์กร
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: a6af617fa4235868f0754ff4c06f4cc73b1700ef14ea449dd1886ab100ddd384
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102290"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>ลบผู้ใช้ที่ถูกไม่มีสิทธิ์ออกจากเซิร์ฟเวอร์ภายในองค์กร

เมื่อต้องการเอาผู้ใช้ที่ถูกไม่มีการเชื่อมโยงออก ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. บังคับการซิงโครไนซ์ไดเรกทอรีโดยปฏิบัติตามคําแ[นะนําใน ข้อมูลเฉพาะตัวแบบAzure Active Directoryคืออะไร](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)

2. เมื่อต้องการตรวจสอบการซิงโครไนซ์ไดเรกทอรี[ให้ดู ข้อมูลเฉพาะตัวแบบไฮบริดAzure Active Directoryคืออะไร](https://technet.microsoft.com/library/jj151797.aspx)

3. ถ้าฟังก์ชันการซิงค์ถูกต้องแล้ว แต่การลบวัตถุ Active Directory ไม่เผยแพร่ไปยัง Azure AD ให้เอาวัตถุที่ไม่มีการเชื่อมโยงออกด้วยตนเองโดยใช้หนึ่งในมอดูล Azure Active Directory ต่อไปนี้Windows PowerShell cmdlets:

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    ตัวอย่างเช่น เมื่อต้องการเอา ID ผู้ใช้ john.smith@contoso.com ออก ซึ่งถูกสร้างขึ้นโดยใช้การซิงโครไนซ์ไดเรกทอรี ให้เรียกใช้ cmdlet

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com