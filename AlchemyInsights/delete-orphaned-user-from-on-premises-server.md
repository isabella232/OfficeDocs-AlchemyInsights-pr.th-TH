---
title: ลบผู้ใช้ที่ไม่ได้ใช้งานจากเซิร์ฟเวอร์ภายในองค์กร
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
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680154"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>ลบผู้ใช้ที่ไม่ได้ใช้งานจากเซิร์ฟเวอร์ภายในองค์กร

เมื่อต้องการลบผู้ใช้ที่ไม่ได้ใช้งานให้ทำตามขั้นตอนต่อไปนี้:

1. บังคับการซิงโครไนซ์ไดเรกทอรีโดยทำตามคำแนะนำใน[ข้อมูลเฉพาะตัวของไฮบริดที่มี Azure Active directory ใช่หรือไม่](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)

2. เมื่อต้องการตรวจสอบการซิงโครไนซ์ไดเรกทอรีให้ดู[ที่ข้อมูลเฉพาะตัวแบบไฮบริดที่มี Azure Active directory คืออะไร](https://technet.microsoft.com/library/jj151797.aspx)

3. ถ้าการซิงค์ฟังก์ชันอย่างถูกต้องแต่การลบวัตถุไดเรกทอรีที่ใช้งานอยู่ไม่ได้เผยแพร่ไปยัง Azure AD ด้วยตนเองให้เอาวัตถุ orphaned ออกโดยใช้โมดูลของ Active Directory ของ Azure สำหรับ cmdlet ของ Windows PowerShell อย่างใดอย่างหนึ่งดังต่อไปนี้

    เอาออก-MsolContact  
    เอาออก-MsolGroup  
    เอาออก-MsolUser

    ตัวอย่างเช่นเมื่อต้องการเอา ID ผู้ใช้ที่ไม่ได้ใช้งาน john.smith@contoso.com ออกโดยใช้การซิงโครไนซ์ไดเรกทอรีให้เรียกใช้ cmdlet ดังนี้

    เอาออก-MsolUser – UserPrincipalName John.Smith@Contoso.com