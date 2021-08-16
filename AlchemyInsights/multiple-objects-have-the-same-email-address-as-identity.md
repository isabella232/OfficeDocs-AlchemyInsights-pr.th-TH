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
ms.openlocfilehash: 5866d182cb2e97e37bc6df87e05fb6ef55bfed1d36f9daa95b7b8993a509e2dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011931"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>วัตถุหลายวัตถุมีที่อยู่อีเมลเดียวกันกับข้อมูลเฉพาะตัว

**วัตถุหลายวัตถุ**

สาเหตุทั่วไปของข้อผิดพลาดนี้ไม่สามารถระบุเส้นทางการร้องขอ Outlook Web Access ได้อย่างถูกต้องเมื่อมีวัตถุหลายวัตถุที่มีที่อยู่อีเมลเดียวกันกับข้อมูลเฉพาะตัว เมื่อต้องการค้นหาวัตถุเหล่านี้ ให้เรียกใช้สั่งต่อไปนี้:

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -โฟลเดอร์สาธารณะ

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

เมื่อต้องการแก้ไขปัญหา ให้เอาวัตถุหลายรายการที่มีข้อมูลเฉพาะตัวอีเมลเดียวกันออก และตรวจสอบให้แน่ใจว่ามีวัตถุเดี่ยวที่มีข้อมูลเฉพาะตัวเฉพาะของอีเมล และชนิดผู้รับคือ UserMailbox

**ที่อยู่เดียวกันจะถูกใช้กับกล่องจดหมายธุรกิจและผู้บริโภค**

อีกสาเหตุหนึ่งคือ เมื่อใช้ที่อยู่เดียวกันนี้กับกล่องจดหมายทางธุรกิจและผู้บริโภค ในกรณีนี้ ผู้ใช้ต้องเปลี่ยนนามแฝงผู้บริโภคหลักของตนจนกว่า Cafe จะสนับสนุนสถานการณ์นี้ นี่คือข้อผิดพลาดถาวรที่ไม่หายไปโดยไม่มีการขัดจังหวะ

หากต้องการรายละเอียด [โปรดดูที่ เปลี่ยนอีเมลแอดเดรสหรือหมายเลขโทรศัพท์ของบัญชี Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)ของคุณ