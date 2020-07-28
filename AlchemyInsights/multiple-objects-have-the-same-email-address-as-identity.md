---
title: วัตถุหลายวัตถุมีที่อยู่อีเมลเดียวกันกับข้อมูลประจําตัว
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439708"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>วัตถุหลายวัตถุมีที่อยู่อีเมลเดียวกันกับข้อมูลประจําตัว

**วัตถุหลายวัตถุ**

หนึ่งในสาเหตุทั่วไปของข้อผิดพลาดนี้จะไม่สามารถกําหนดเส้นทางการร้องขอ Outlook Web Access ได้อย่างถูกต้องในสถานะการมีอยู่ของวัตถุหลายวัตถุที่มีที่อยู่อีเมลเดียวกันเป็นข้อมูลประจําตัว เมื่อต้องการค้นหาวัตถุเหล่านี้ ให้เรียกใช้คําสั่งต่อไปนี้:

· รับผู้รับ<email address>

· รับผู้ใช้<email address>

· รับผู้ใช้ <email address> -SoftDeletedUser

· ติดต่อรับ<email address>

· รับกล่องจดหมาย <email address> -PublicFolder

· รับกล่องจดหมาย <email address> -รวมรวมการติดแท็ก

· รับกล่องจดหมาย <email address> -ไม่ได้ใช้งานกล่องจดหมายเดียว

เมื่อต้องการแก้ไขปัญหา ลบวัตถุหลายวัตถุ ด้วยรหัสประจําตัวอีเมลเดียวกัน และให้แน่ใจว่า ไม่มีวัตถุเดียว กับรหัสประจําตัวอีเมลเฉพาะ และว่า ชนิดผู้รับเป็น UserMailbox

**ที่อยู่เดียวกันจะใช้สําหรับกล่องจดหมายของธุรกิจและผู้บริโภค**

สาเหตุก็คือเมื่อมีใช้ที่อยู่เดียวกันสําหรับธุรกิจและกล่องจดหมายของผู้บริโภค ในกรณีนี้ ผู้ใช้ต้องเปลี่ยนนามแฝงของผู้บริโภคหลักจนกว่า Cafe สนับสนุนสถานการณ์สมมตินี้ นี่คือข้อผิดพลาดถาวรที่ไม่หายไปโดยไม่มีการแทรกแซง

โปรดดูรายละเอียดที่[เปลี่ยนที่อยู่อีเมลหรือหมายเลขโทรศัพท์สําหรับบัญชี Microsoft ของคุณ](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)