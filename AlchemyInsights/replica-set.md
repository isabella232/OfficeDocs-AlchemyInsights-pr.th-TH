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
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714586"
---
# <a name="replica-set"></a>ชุดแบบสมาพ

AADDS จะเรียกว่าโดเมนที่มีการจัดการ จริงๆ แล้วคือตัวควบคุมโดเมนสองตัวที่เรียกใช้และดูแลรักษาโดย Backend DCs สองเครื่องจะมีหนึ่ง DC หลักและหนึ่งการซ้อแบบ DC การสํารองข้อมูลใน AADDS (โดเมนที่มีการจัดการ) เป็นกระบวนการอัตโนมัติที่จัดการโดยแพลตฟอร์ม Azure การสนับสนุน Azure สามารถช่วยคุณคืนค่าจากการสํารองข้อมูลในกรณีที่เกิดปัญหากับโดเมนที่มีการจัดการของคุณ

คุณสร้างชุดแบบเสมือนแต่ละชุดในเครือข่ายเสมือน เครือข่ายเสมือนแต่ละเครือข่ายต้องถูกเพียร์กับเครือข่ายเสมือนอื่นๆ ที่โฮสต์ชุดแบบพรีวิวของโดเมนที่มีการจัดการ การกําหนดค่านี้สร้างโทโพโลยีเครือข่ายตาข่ายที่สนับสนุนการกําหนดค่าไดเรกทอรี เครือข่ายเสมือนสามารถรองรับชุดแบบเสมือนหลายชุดได้ ถ้าชุดแบบเสมือนแต่ละชุดอยู่ในเครือข่ายย่อยเสมือนที่ต่างกัน

For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
