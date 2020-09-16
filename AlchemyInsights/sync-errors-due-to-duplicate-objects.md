---
title: ๙๐๒ (ข้อผิดพลาดในการซิงค์เนื่องจากวัตถุที่ซ้ำกัน)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737360"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>ข้อผิดพลาดการซิงค์เนื่องจากวัตถุที่ซ้ำกัน

คุณอาจได้รับข้อความแสดงข้อผิดพลาดอย่างใดอย่างหนึ่งต่อไปนี้เมื่อซิงโครไนซ์ไดเรกทอรีเสร็จสิ้นใน Microsoft ๓๖๕:

- ไม่สามารถปรับปรุงวัตถุนี้ในบริการ Microsoft Online ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เกี่ยวข้องกับวัตถุนี้มีค่าที่อาจเกี่ยวข้องกับวัตถุอื่นในไดเรกทอรีภายในเครื่องของคุณแล้ว

- วัตถุที่ซิงโครไนซ์ที่มีที่อยู่พร็อกซีเดียวกันมีอยู่แล้วในไดเรกทอรี Microsoft Online Services ของคุณ

- ไม่สามารถอัปเดอ็อบเจกต์นี้ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เกี่ยวข้องกับวัตถุนี้มีค่าที่อาจเกี่ยวข้องกับวัตถุอื่นในบริการไดเรกทอรีภายในเครื่องของคุณ: UserPrincipalName

เมื่อต้องการระบุและแก้ไขปัญหาให้ดาวน์โหลดและเรียกใช้[เครื่องมือการแก้ไขข้อผิดพลาดของ IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832)

สำหรับข้อมูลเพิ่มเติมให้ดูที่[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
