---
title: Yammerเกี่ยวกับการให้สิทธิ์การใช้งาน
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
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989754"
---
# <a name="yammer-licensing-issues"></a>Yammerเกี่ยวกับการให้สิทธิ์การใช้งาน

ผู้ใช้ทั้งหมดต้องมีสิทธิ์การใช้งานเพื่อใช้บริการ Yammer Enterprise แต่ตามค่าเริ่มต้น Yammerไม่ต้องการให้ผู้ใช้มีสิทธิ์การใช้งานเพื่อเข้าถึงบริการ เมื่อผู้ดูแลระบบเปลี่ยนแปลงการตั้งค่าเพื่อบล็อกMicrosoft 365ผู้ใช้Yammerผู้ใช้ที่ไม่มีสิทธิ์การใช้งาน Yammer Enterprise สิทธิ์จะไม่สามารถเข้าถึงบริการ Yammerได้ For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

เมื่อเอาสิทธิ์การใช้งานออกจากผู้ใช้ ไทล์Yammerจะไม่แสดงอีกต่อไป และบริการอื่นๆ สามารถใช้การเอาสิทธิ์การใช้งานออกเพื่อซ่อนฟีเจอร์ ในกรณีอื่น ฟีเจอร์ยังคงสามารถปรากฏได้ แต่ต้องมีการมอบหมายสิทธิ์การใช้งานเพื่อดําเนินการ  

**สิทธิ์การใช้งานไม่ได้รับการอัปเดตให้กับผู้ใช้**  

ในบางครั้ง ผู้ใช้จะถูกมอบหมายสิทธิ์การใช้งาน แต่ยังไม่สามารถเข้าถึงYammerได้ ความล่าช้าอาจเกิดขึ้นเมื่ออยู่ระหว่างการมอบหมายสิทธิ์การใช้งานหลายสิทธิ์ Yammerผู้ใช้อาจไม่ถูกอัปเดตในลดับเดียวกับที่มีการเปลี่ยนสิทธิ์การใช้งานใน Azure AD เนื่องจากระบบจะเรียกใช้แบบอะซิงโครนัส รอถึง 24 ชั่วโมงก่อนที่จะเปิดกรณีการสนับสนุนเพื่อรายงานปัญหาการซิงค์สิทธิ์การใช้งาน  

**การมอบหมายสิทธิ์การใช้งานเป็นกลุ่ม**  

คุณสามารถมอบหมายสิทธิ์การใช้งานผ่านศูนย์การจัดการหรือการเขียนสคริปต์ PowerShell For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and Assign [licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

ฝ่ายสนับสนุนของ Microsoft ไม่มีความช่วยเหลือในการสร้างสคริปต์ แต่เอกสารประกอบเกี่ยวกับYammerสิทธิ์การใช้งานที่พร้อมใช้งาน ดูข้อมูลเพิ่มเติมได้ที่ จัดการ[Yammerการใช้งานของคุณWindows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)