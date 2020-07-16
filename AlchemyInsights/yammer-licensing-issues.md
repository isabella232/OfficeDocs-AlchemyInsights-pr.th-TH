---
title: ปัญหาการอนุญาตให้ใช้สิทธิ์ Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148426"
---
# <a name="yammer-licensing-issues"></a>ปัญหาการอนุญาตให้ใช้สิทธิ์ Yammer

ผู้ใช้ทั้งหมดต้องมีสิทธิ์การใช้งานเพื่อใช้บริการ Yammer องค์กร แต่โดยค่าเริ่มต้น Yammer ไม่จําเป็นต้องให้ผู้ใช้มีสิทธิ์การใช้งานในการเข้าถึงบริการ เมื่อผู้ดูแลระบบเปลี่ยนแปลงการตั้งค่าเพื่อบล็อกผู้ใช้ Microsoft 365 โดยไม่มีสิทธิ์การใช้งาน Yammer ผู้ใช้ไม่ได้กําหนดสิทธิ์การใช้งาน Yammer องค์กรไม่สามารถเข้าถึงบริการ Yammer สําหรับข้อมูลเพิ่มเติม ให้ดูที่[จัดการสิทธิ์การใช้งานของผู้ใช้ Yammer ใน Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

เมื่อสิทธิ์การใช้งานจะถูกเอาออกจากผู้ใช้ จะไม่มีแสดงไทล์ Yammer อีกต่อไป และบริการอื่น ๆ สามารถใช้การเอาออกสิทธิ์การใช้งานเพื่อซ่อนลักษณะการทํางาน ในกรณีอื่นๆ ฟีเจอร์ยังคงปรากฏอยู่ แต่จําเป็นต้องมีการกําหนดสิทธิ์การใช้งานเพื่อใช้งาน  

**สิทธิ์การใช้งานไม่ได้รับการปรับปรุงสําหรับผู้ใช้**  

ในบางครั้ง ผู้ใช้จะได้รับมอบหมายสิทธิ์การใช้งาน แต่ยังคงไม่สามารถเข้าถึง Yammer ได้ ความล่าช้ามีแนวโน้มที่จะเกิดขึ้นเมื่อการมอบหมายใบอนุญาตจํานวนมากกําลังดําเนินการ ผู้ใช้ Yammer อาจไม่ได้รับการปรับปรุงในลําดับเดียวกันเป็นสิทธิ์การใช้งานมีการเปลี่ยนแปลงในโฆษณา Azure เนื่องจากระบบทํางานแบบอะซิงโครนัส รอถึง 24 ชั่วโมงก่อนที่จะเปิดกรณีการสนับสนุนเพื่อรายงานปัญหาการซิงค์ใบอนุญาต  

**การมอบหมายสิทธิ์การใช้งานจํานวนมาก**  

สิทธิ์การใช้งานสามารถถูกกําหนดผ่านศูนย์การจัดการหรือการเขียนสคริปต์ PowerShell สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การกําหนดสิทธิ์การใช้งานให้กับผู้ใช้](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)และ[มอบหมายสิทธิ์การใช้งานให้กับบัญชีผู้ใช้ด้วย Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

ฝ่ายสนับสนุนของ Microsoft ไม่ได้ให้ความช่วยเหลือในการสร้างสคริปต์ แต่เอกสารเกี่ยวกับการกําหนดสิทธิ์การใช้งาน Yammer จะพร้อมใช้งาน สําหรับข้อมูลเพิ่มเติม ให้ดูที่[จัดการสิทธิ์การใช้งาน Yammer โดยใช้ Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)