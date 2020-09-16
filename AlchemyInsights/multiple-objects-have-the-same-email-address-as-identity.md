---
title: วัตถุหลายวัตถุมีที่อยู่อีเมลเดียวกันกับข้อมูลเฉพาะตัว
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724634"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>วัตถุหลายวัตถุมีที่อยู่อีเมลเดียวกันกับข้อมูลเฉพาะตัว

**วัตถุหลายวัตถุ**

หนึ่งในสาเหตุทั่วไปของข้อผิดพลาดนี้ไม่สามารถกำหนดเส้นทางการร้องขอการเข้าถึงเว็บ Outlook อย่างถูกต้องในการแสดงตนของวัตถุหลายวัตถุที่มีที่อยู่อีเมลเดียวกันกับข้อมูลเฉพาะตัว เมื่อต้องการค้นหาวัตถุเหล่านี้ให้เรียกใช้คำสั่งต่อไปนี้:

· รับผู้รับ <email address>

· รับผู้ใช้ <email address>

· รับผู้ใช้ <email address> -SoftDeletedUser

· รับที่ติดต่อ <email address>

· รับ-กล่องจดหมาย <email address> -PublicFolder

· รับ-กล่องจดหมาย <email address> -IncludeSoftDeletedMailbox

· รับ-กล่องจดหมาย <email address> -InactiveMailboxOnly

เมื่อต้องการแก้ไขปัญหานี้ให้เอาวัตถุออกหลายวัตถุด้วยข้อมูลเฉพาะตัวอีเมลเดียวกันและตรวจสอบให้แน่ใจว่ามีวัตถุเดียวที่มีข้อมูลเฉพาะตัวของอีเมลที่ระบุและชนิดของผู้รับเป็น UserMailbox

**ใช้ที่อยู่เดียวกันสำหรับกล่องจดหมายธุรกิจและผู้บริโภค**

สาเหตุอีกประการหนึ่งคือเมื่อใช้ที่อยู่เดียวกันสำหรับกล่องจดหมายธุรกิจและผู้บริโภค ในกรณีนี้ผู้ใช้ต้องเปลี่ยนนามแฝงผู้ใช้หลักของพวกเขาจนกว่า Cafe จะสนับสนุนสถานการณ์นี้ นี่เป็นข้อผิดพลาดถาวรที่ไม่หายไปโดยไม่มีการแทรกแซง

สำหรับรายละเอียดให้ดู[ที่เปลี่ยนที่อยู่อีเมลหรือหมายเลขโทรศัพท์สำหรับบัญชี Microsoft ของคุณ](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)