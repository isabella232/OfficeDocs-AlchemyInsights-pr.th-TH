---
title: 902 (ข้อผิดพลาดเนื่องจากวัตถุที่ซ้ำกัน)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493939"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>ข้อผิดพลาดในการซิงค์ได้เนื่องจากวัตถุที่ซ้ำกัน

คุณอาจได้รับข้อความแสดงข้อผิดพลาดต่อไปนี้เมื่อเสร็จสิ้นการซิงโครไนส์ของไดเรกทอรี:
  
- ไม่สามารถปรับปรุงวัตถุนี้ในบริการออนไลน์ของ Microsoft ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เกี่ยวข้องกับวัตถุนี้มีค่าที่มีอยู่แล้วอาจเกี่ยวข้องกับวัตถุอื่นในไดเรกทอรีภายในเครื่องของคุณ
    
- วัตถุทำข้อมูลให้ตรงกับที่อยู่พร็อกซีเดียวกันอยู่แล้วในไดเรกทอรีการบริการแบบออนไลน์ของ Microsoft
    
- ไม่สามารถปรับปรุงวัตถุนี้ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เกี่ยวข้องกับวัตถุนี้มีค่าที่มีอยู่แล้วอาจเกี่ยวข้องกับวัตถุอื่นในบริการไดเรกทอรีภายในเครื่องของคุณ: UserPrincipalName
    
เมื่อต้องการระบุ และแก้ไขปัญหา ดาวน์โหลด และเรียกใช้[เครื่องมือด้านข้อผิดพลาดของ DirSync IdFix](https://www.microsoft.com/download/details.aspx?id=36832)
  
สำหรับข้อมูลเพิ่มเติม ให้ดู[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
  

