---
title: Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049327"
---
# <a name="4c7-error-in-microsoft-teams"></a>ข้อผิดพลาด 4c7 ใน Microsoft Teams

ข้อผิดพลาดนี้เกิดขึ้นเนื่องจากMicrosoft Teamsการรับรองความถูกต้องของฟอร์ม เมื่อคุณปรับใช้ Active Directory Federation Services (AD FS) การรับรองความถูกต้องของฟอร์มจะไม่เปิดใช้งานกับอินทราเน็ตตามค่าเริ่มต้น If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.

เมื่อต้องการแก้ไขปัญหานี้ ให้เปิดใช้งานการรับรองความถูกต้องของฟอร์มโดยใช้ Snap-in ของ AD FS Microsoft Management Console (MMC) บนคอมพิวเตอร์ที่มีสําเนาภายในเครื่องของ Active Directory เมื่อต้องการให้ปฏิบัติตามขั้นตอนเหล่านี้: 

1. ในบานหน้าต่างนําทาง ให้เรียกดู **นโยบายการรับรองความถูกต้อง**
2. ภายใต้ **การ** แอคชัน ในบานหน้าต่างรายละเอียด ให้เลือก แก้ไข **การรับรองความถูกต้องหลัก** ส่วนกลาง
3. บนแท็บ **อินทราเน็ต ให้เลือก****การรับรองความถูกต้องของฟอร์ม**
4. เลือก **ตกลง** (หรือ **Apply**)