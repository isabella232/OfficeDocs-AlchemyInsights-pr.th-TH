---
title: ไม่ได้Outlookป้ายผนึกเริ่มต้น
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/17/2021
ms.locfileid: "58455084"
---
# <a name="default-outlook-label-setting-not-applied"></a>ไม่ได้Outlookป้ายผนึกเริ่มต้น

ถ้าการตั้งค่าป้ายชื่อเริ่มต้นของ Outlook ของคุณใช้ไม่ได้อย่างถูกต้อง และป้ายชื่ออื่นหรือไม่มีป้ายชื่อใดถูกใช้งาน คุณอาจประสบปัญหาที่ทราบแล้ว (MC277818) และควรเลือกตัวเลือกใดตัวเลือกหนึ่งใน 2 ตัวเลือกเหล่านี้เพื่อแก้ไขปัญหา:

**ตัวเลือกที่ 1:**

1. ไปที่ ศูนย์Microsoft 365การปฏิบัติตาม>**โซลูชัน**  >  **การป้องกัน** ข้อมูล
1. เลือก **นโยบาย** ป้ายชื่อ แล้วเลือกนโยบายป้ายชื่อที่คุณต้องการแก้ไข ( การตั้งค่า **OutlookDefaultlabel** ไม่ได้ตั้งค่าอย่างถูกต้องบนนโยบายป้ายชื่อในคําถาม เรียกใช้ **Get-labelpolicy** เพื่อดูการตั้งค่านี้) แล้วเลือก **แก้ไข** นโยบาย
1. **เลือก** ถัดไป จนกว่าคุณจะเห็นการตั้งค่าใช้ป้ายชื่อเริ่มต้นนี้กับอีเมล ซึ่งพร้อมใช้งานถ้าคุณเลือก ต้องให้ผู้ใช้ใช้ป้ายชื่อกับอีเมลและเอกสารที่ทายาท ในกล่องโต้ตอบ **การตั้งค่า** นโยบาย
1. ในกล่องโต้ตอบ **ใช้ป้ายชื่อเริ่มต้นกับเอกสาร** ให้เลือก **ไม่มี** จากรายการดรอปดาวน์
1. เลือก **ถัดไป** แล้ว **ส่ง** เพื่อบันทึกการตั้งค่าป้ายชื่อของคุณ

**ตัวเลือกที่ 2:**

ใน [Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)ของศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย ให้ใช้ commandlet Set-LabelPolicy เพื่อเปลี่ยน **OutlookDefaultlabel** **เป็น None** บน {OutlookDefaultLabel="None"}

เรียกใช้: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

For more information on default labels for Outlook, see [Set a different default label for Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).