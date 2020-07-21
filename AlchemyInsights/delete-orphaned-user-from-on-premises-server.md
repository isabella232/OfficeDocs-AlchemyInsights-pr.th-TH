---
title: ลบผู้ใช้ที่ถูกละเลยจากเซิร์ฟเวอร์ในสถาน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198585"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>ลบผู้ใช้ที่ถูกละเลยจากเซิร์ฟเวอร์ในสถาน

เมื่อต้องการเอาผู้ใช้ที่ไม่ได้ใช้งาน ให้ทําตามขั้นตอนเหล่านี้:

1. บังคับให้ซิงโครไนส์ไดเรกทอรี โดยทําตามคําแนะนําใน[รหัสประจําตัวไฮบริดสลีกับไดเรกทอรีที่ใช้งานอยู่ของ Azure คืออะไร](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)

2. เมื่อต้องการตรวจสอบการซิงโครไนส์ไดเรกทอรี ให้ดูที่[รหัสประจําตัวไฮบริดสลีกับไดเรกทอรีที่ใช้งานอยู่ของ Azure คืออะไร](https://technet.microsoft.com/library/jj151797.aspx)

3. ถ้าฟังก์ชันซิงค์อย่างถูกต้อง แต่การลบวัตถุไดเรกทอรีที่ใช้งานอยู่ไม่เผยแพร่ไปยังโฆษณา Azure ด้วยตนเองเอาวัตถุที่ถูกละเลย โดยใช้ต่อไปนี้ Azure Active Directory โมดูลสําหรับ Windows PowerShell cmdlets:

    ลบ- msolติดต่อ  
    ลบ- Msolกรุ๊ป  
    ลบ- msolUser

    ตัวอย่างเช่น เมื่อต้องการเอา id ผู้ใช้ที่ถูกjohn.smith@contoso.com orphaned ที่สร้างโดยใช้การซิงโครไนส์ของไดเรกทอรี เรียกใช้ cmdlet:

    ลบ - MsolUser - UserPrincipalname John.Smith@Contoso.com