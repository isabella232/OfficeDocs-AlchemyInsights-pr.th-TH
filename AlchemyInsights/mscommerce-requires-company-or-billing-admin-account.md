---
title: เชื่อมต่อกับมอดูล MSCommerce
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829755"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce ต้องใช้บัญชีของบริษัทหรือผู้ดูแลการเรียกเก็บเงิน

โมดูล MSCommerce ต้องใช้บัญชีที่มีสิทธิ์ผู้ดูแลระบบของบริษัทหรือผู้ดูแลการเรียกเก็บเงิน ถ้าคุณได้รับข้อผิดพลาดต่อไปนี้ คุณจะต้องเชื่อมต่อกับบัญชีอื่นอีกครั้ง

*ErrorMessage - เซิร์ฟเวอร์ระยะไกลส่งกลับข้อผิดพลาด: (403) Forbidden ErrorDetails - ที่ C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "ไม่สามารถลองใหม่...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : ไม่ระบุ: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

ถ้าบัญชีของคุณไม่มีสิทธิ์ผู้ดูแลระบบของบริษัทหรือผู้ดูแลการเรียกเก็บเงิน ให้ติดต่อผู้ดูแลระบบ IT ของคุณ
