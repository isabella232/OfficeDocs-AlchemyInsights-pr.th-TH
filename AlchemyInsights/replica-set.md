---
title: ชุดแบบสมาพ
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110699"
---
# <a name="replica-set"></a>ชุดแบบสมาพ

AADDS จะเรียกอีกอย่างว่าโดเมนที่มีการจัดการ จริงๆ แล้วตัวควบคุมโดเมนสองตัวที่เรียกใช้และดูแลรักษาโดย Backend DCs สอง DCs มีหนึ่ง DC หลักและหนึ่งการซ้กแบบ DC การสํารองข้อมูลใน AADDS (โดเมนที่มีการจัดการ) เป็นกระบวนการอัตโนมัติที่จัดการโดยแพลตฟอร์ม Azure ในกรณีที่เกิดปัญหากับโดเมนที่มีการจัดการ การสนับสนุน Azure สามารถช่วยคุณคืนค่าจากการสํารองข้อมูลได้

คุณสร้างชุดแบบเสมือนแต่ละชุดในเครือข่ายเสมือน เครือข่ายเสมือนแต่ละเครือข่ายต้องถูกเพียร์ไปยังเครือข่ายเสมือนอื่นๆ ที่โฮสต์ชุดแบบเสมือนของโดเมนที่มีการจัดการ การกําหนดค่านี้สร้างโทโพโลยีเครือข่ายตาข่ายที่สนับสนุนการกําหนดค่าไดเรกทอรี เครือข่ายเสมือนสามารถสนับสนุนชุดแบบเสมือนหลายชุด ถ้าแต่ละชุดแบบเสมือนอยู่ในเครือข่ายย่อยเสมือนที่ต่างกัน

For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
