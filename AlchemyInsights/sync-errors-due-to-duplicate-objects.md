---
title: 902 (ข้อผิดพลาดในการซิงค์เนื่องจากวัตถุที่ซ้้ากัน)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998819"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>การซิงค์ข้อผิดพลาดเนื่องจากวัตถุที่คัดลอก

คุณอาจได้รับข้อความแสดงข้อผิดพลาดอย่างใดอย่างหนึ่งต่อไปนี้ เมื่อการซิงโครไนซ์ไดเรกทอรีเสร็จสิ้นMicrosoft 365:

- ไม่สามารถอัปเดตวัตถุนี้ใน Microsoft Online Services ได้ เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เชื่อมโยงกับวัตถุนี้มีค่าที่อาจเชื่อมโยงกับวัตถุอื่นในไดเรกทอรีภายในเครื่องของคุณอยู่แล้ว

- วัตถุที่ซิงโครไนซ์กับที่อยู่พร็อกซีเดียวกันมีอยู่แล้วในไดเรกทอรี Microsoft Online Services ของคุณ

- ไม่สามารถอัปเดตวัตถุนี้ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เชื่อมโยงกับวัตถุนี้มีค่าที่อาจเชื่อมโยงกับวัตถุอื่นอยู่แล้วในบริการไดเรกทอรีภายในของคุณ: UserPrincipalName

เมื่อต้องการระบุและแก้ไขปัญหา ให้ดาวน์โหลดและเรียกใช้เครื่องมือแก้ไขปัญหาข้อผิดพลาด[IdFix DirSync](https://github.com/Microsoft/idfix)

For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
