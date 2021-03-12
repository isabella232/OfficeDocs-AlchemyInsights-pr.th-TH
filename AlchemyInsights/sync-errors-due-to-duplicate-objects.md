---
title: 902 (ข้อผิดพลาดในการซิงค์เนื่องจากวัตถุที่ซ้ากัน)
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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708081"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>การซิงค์ข้อผิดพลาดเนื่องจากวัตถุที่คัดลอกกัน

คุณอาจได้รับข้อความแสดงข้อผิดพลาดต่อไปนี้เมื่อการซิงโครไนซ์ไดเรกทอรีเสร็จสิ้นใน Microsoft 365:

- ไม่สามารถอัปเดตวัตถุนี้ใน Microsoft Online Services ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เชื่อมโยงกับวัตถุนี้มีค่าที่อาจเชื่อมโยงกับวัตถุอื่นในไดเรกทอรีภายในเครื่องของคุณอยู่แล้ว

- วัตถุที่ซิงโครไนซ์ที่มีที่อยู่พร็อกซีเดียวกันมีอยู่แล้วในไดเรกทอรี Microsoft Online Services ของคุณ

- ไม่สามารถอัปเดตวัตถุนี้ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เชื่อมโยงกับวัตถุนี้มีค่าที่อาจเชื่อมโยงกับวัตถุอื่นในบริการไดเรกทอรีภายในของคุณอยู่แล้ว: UserPrincipalName

เมื่อต้องการระบุและแก้ไขปัญหา ให้ดาวน์โหลดและเรียกใช้เครื่องมือแก้ไขปัญหาข้อผิดพลาด[IdFix DirSync](https://github.com/Microsoft/idfix)

For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
