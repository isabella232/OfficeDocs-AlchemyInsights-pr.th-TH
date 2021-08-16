---
title: ระบุWindowsเดสก์ท็อปเสมือน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 398496448089d4480119a2eb21221dc11f13c6c1f3bcbd931d6c18033f2e734e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53987588"
---
# <a name="identify-windows-virtual-desktop-issues"></a>ระบุWindowsเดสก์ท็อปเสมือน

Windows การวินิจฉัยเดสก์ท็อปเสมือนใช้ cmdlet PowerShell เพียงรายการเดียว แต่ประกอบด้วยพารามิเตอร์เพิ่มเติมมากมายเพื่อช่วยลดขอบเขตและแยกปัญหา เมื่อต้องการเริ่มต้นใช้งาน: 

1. ดาวน์โหลดและนําเข้าWindowsโมดูล PowerShell บนเดสก์ท็อปเสมือน For details, see [Windows Virtual Desktop cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. เรียกใช้ cmdlet ต่อไปนี้เพื่อลงชื่อเข้าใช้บัญชีของคุณ:
    
    ตัวอย่าง: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**หมายเหตุ:** คิวรีทั้งหมดที่ใช้ PowerShell ต้องมีพารามิเตอร์ -UserName หรือ -ActivityID หากต้องการความสามารถในการตรวจสอบ โปรดดู [ใช้ Log Analytics เพื่อดูฟีเจอร์](https://go.microsoft.com/fwlink/?linkid=2126847)การวินิจฉัย

เมื่อต้องการกรองกิจกรรมการวินิจฉัยโดยผู้ใช้ ให้เรียกใช้ cmdlet ต่อไปนี้:

ตัวอย่าง: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

มีรายการตัวกรองที่คุณสามารถเรียกใช้เพื่อวินิจฉัยปัญหา เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการวินิจฉัยปัญหา ให้ดู[ระบุและวินิจฉัยWindowsเดสก์ท็อปเสมือน](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับข้อผิดพลาดทั่วไป ให้ดูที่[เซตารีโอข้อผิดพลาดทั่วไป](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)
