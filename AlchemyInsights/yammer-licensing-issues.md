---
title: ปัญหาสิทธิ์การใช้งาน Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657295"
---
# <a name="yammer-licensing-issues"></a>ปัญหาสิทธิ์การใช้งาน Yammer

ผู้ใช้ทุกคนต้องมีสิทธิ์การใช้งานในการใช้บริการ Yammer Enterprise แต่ตามค่าเริ่มต้น Yammer ไม่จำเป็นต้องมีสิทธิ์การใช้งานในการเข้าถึงบริการ เมื่อผู้ดูแลระบบเปลี่ยนการตั้งค่าเพื่อบล็อกผู้ใช้ Microsoft ๓๖๕โดยไม่มีสิทธิ์การใช้งาน Yammer ผู้ใช้ที่ไม่ได้กำหนดสิทธิ์การใช้งาน Yammer Enterprise ไม่สามารถเข้าถึงบริการ Yammer ได้ สำหรับข้อมูลเพิ่มเติมให้ดู [ที่จัดการสิทธิ์การใช้งานของผู้ใช้ Yammer ใน Office ๓๖๕](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

เมื่อสิทธิ์การใช้งานถูกเอาออกจากผู้ใช้ไทล์ Yammer จะไม่แสดงอีกต่อไปและบริการอื่นๆสามารถใช้สิทธิ์การเอาสิทธิ์การใช้งานเพื่อซ่อนฟีเจอร์ได้อีกต่อไป ในกรณีอื่นๆฟีเจอร์ยังสามารถปรากฏขึ้นได้แต่จำเป็นต้องมีการมอบหมายสิทธิ์การใช้งานเพื่อดำเนินการ  

**สิทธิ์การใช้งานไม่ได้รับการอัปเดตสำหรับผู้ใช้**  

ในบางครั้งผู้ใช้จะได้รับมอบหมายสิทธิ์การใช้งานแต่ยังไม่สามารถเข้าถึง Yammer ได้ ความล่าช้ามีแนวโน้มที่จะเกิดขึ้นเมื่อมีการกำหนดสิทธิ์การใช้งานจำนวนมากกำลังดำเนินการอยู่ ผู้ใช้ Yammer อาจไม่ได้รับการอัปเดตในลำดับเดียวกันกับสิทธิ์การใช้งานที่มีการเปลี่ยนแปลงใน Azure AD เนื่องจากระบบทำงานแบบอะซิงโครนัส รอจนถึง24ชั่วโมงก่อนที่จะเปิดกรณีสนับสนุนเพื่อรายงานปัญหาการซิงค์สิทธิ์การใช้งาน  

**การมอบหมายสิทธิ์การเป็นกลุ่มจำนวนมาก**  

สิทธิ์การใช้งานสามารถกำหนดได้ผ่านทางศูนย์การจัดการหรือการเขียนสคริปต์ PowerShell สำหรับข้อมูลเพิ่มเติมให้ดู[ที่กำหนดสิทธิ์การใช้งานให้กับผู้ใช้](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)และ[กำหนดสิทธิ์การใช้งานให้กับบัญชีผู้ใช้ด้วย Office ๓๖๕ PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

ฝ่ายสนับสนุนของไมโครซอฟท์ไม่มีความช่วยเหลือเกี่ยวกับการสร้างสคริปต์แต่เอกสารประกอบบนการกำหนดสิทธิ์การใช้งาน Yammer จะพร้อมใช้งาน สำหรับข้อมูลเพิ่มเติมให้ดูที่[จัดการสิทธิ์การใช้งาน Yammer โดยใช้ Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)