---
title: ระบุปัญหาเดสก์ท็อปเสมือนของ Windows
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
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596036"
---
# <a name="identify-windows-virtual-desktop-issues"></a>ระบุปัญหาเดสก์ท็อปเสมือนของ Windows

การวินิจฉัยเดสก์ท็อปเสมือนของ Windows ใช้ cmdlet ของ PowerShell เพียงรายการเดียว แต่ประกอบด้วยพารามิเตอร์เพิ่มเติมมากมายเพื่อช่วยลดและแยกปัญหา เมื่อต้องการเริ่มต้นใช้งาน: 

1. ดาวน์โหลดและนําเข้ามอดูล PowerShell บนเดสก์ท็อปเสมือนของ Windows For details, see [Windows Virtual Desktop cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. เรียกใช้ cmdlet ต่อไปนี้เพื่อลงชื่อเข้าใช้บัญชีของคุณ:
    
    ตัวอย่าง: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**หมายเหตุ:** คิวรีทั้งหมดที่ใช้ PowerShell ต้องมีพารามิเตอร์ -UserName หรือ -ActivityID ดูการใช้ Log Analytics เพื่อดูฟีเจอร์การวินิจฉัยเพื่อดู[ความสามารถในการตรวจสอบ](https://go.microsoft.com/fwlink/?linkid=2126847)

เมื่อต้องการกรองกิจกรรมการวินิจฉัยโดยผู้ใช้ ให้เรียกใช้ cmdlet ต่อไปนี้:

ตัวอย่าง: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

มีรายการตัวกรองที่คุณสามารถเรียกใช้เพื่อวินิจฉัยปัญหา เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการวินิจฉัยปัญหา ให้ดู ระบุ[และวินิจฉัยปัญหาเดสก์ท็อปเสมือนของ Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับข้อผิดพลาดทั่วไป ให้ดูที่ [เซนารีข้อผิดพลาด](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)ทั่วไป
