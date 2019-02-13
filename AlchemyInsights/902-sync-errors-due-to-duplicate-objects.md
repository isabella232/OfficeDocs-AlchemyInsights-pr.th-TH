---
title: 902 (ข้อผิดพลาดเนื่องจากวัตถุที่ซ้ำกัน)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f576460547110e0e599a9062ae03f690792fe635
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919891"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>ข้อผิดพลาดในการซิงค์ได้เนื่องจากวัตถุที่ซ้ำกัน

คุณอาจได้รับข้อความแสดงข้อผิดพลาดต่อไปนี้เมื่อเสร็จสิ้นการซิงโครไนส์ของไดเรกทอรี:
  
- ไม่สามารถปรับปรุงวัตถุนี้ในบริการออนไลน์ของ Microsoft ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เกี่ยวข้องกับวัตถุนี้มีค่าที่มีอยู่แล้วอาจเกี่ยวข้องกับวัตถุอื่นในไดเรกทอรีภายในเครื่องของคุณ
    
- วัตถุทำข้อมูลให้ตรงกับที่อยู่พร็อกซีเดียวกันอยู่แล้วในไดเรกทอรีการบริการแบบออนไลน์ของ Microsoft
    
- ไม่สามารถปรับปรุงวัตถุนี้ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เกี่ยวข้องกับวัตถุนี้มีค่าที่มีอยู่แล้วอาจเกี่ยวข้องกับวัตถุอื่นในบริการไดเรกทอรีภายในเครื่องของคุณ: UserPrincipalName
    
เมื่อต้องการระบุ และแก้ไขปัญหา ดาวน์โหลด และเรียกใช้[เครื่องมือด้านข้อผิดพลาดของ DirSync IdFix](https://www.microsoft.com/download/details.aspx?id=36832)
  
สำหรับข้อมูลเพิ่มเติม ให้ดู[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
  

