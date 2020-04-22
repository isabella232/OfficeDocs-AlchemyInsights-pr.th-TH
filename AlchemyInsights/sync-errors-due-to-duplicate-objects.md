---
title: 902 (ข้อผิดพลาดในการซิงค์เนื่องจากวัตถุที่ซ้ํากัน)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767159"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>ข้อผิดพลาดในการซิงค์เนื่องจากวัตถุที่ซ้ํากัน

คุณอาจได้รับข้อความแสดงข้อผิดพลาดต่อไปนี้อย่างใดอย่างหนึ่งเมื่อซิงโครไนส์ไดเรกทอรีเสร็จสิ้นใน Microsoft 365:

- ไม่สามารถปรับปรุงวัตถุนี้ในบริการแบบออนไลน์ของ Microsoft ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เกี่ยวข้องกับวัตถุนี้มีค่าที่อาจเชื่อมโยงกับวัตถุอื่นในไดเรกทอรีภายในเครื่องของคุณ

- มีวัตถุที่ซิงโครไนส์กับที่อยู่พร็อกซีเดียวกันอยู่แล้วในไดเรกทอรีบริการออนไลน์ของ Microsoft

- ไม่สามารถปรับปรุงวัตถุนี้ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เกี่ยวข้องกับวัตถุนี้มีค่าที่อาจเชื่อมโยงกับวัตถุอื่นในบริการไดเรกทอรีภายในเครื่องของคุณ: UserPrincipalName

เมื่อต้องการระบุและแก้ไขปัญหา ให้ดาวน์โหลดและเรียกใช้[เครื่องมือแก้ไขข้อผิดพลาด DirSync IdFix](https://www.microsoft.com/download/details.aspx?id=36832)

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
