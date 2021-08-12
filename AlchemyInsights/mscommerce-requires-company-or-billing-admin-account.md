---
title: เชื่อมต่อไปยังมอดูล MSCommerce
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
ms.openlocfilehash: 357604f1d4cda3ac8ef6b8b4dbf8780b96dcee59409a6c2edad4a84d6adda62a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974692"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce ต้องใช้บัญชีของบริษัทหรือผู้ดูแลการเรียกเก็บเงิน

โมดูล MSCommerce ต้องใช้บัญชีที่มีสิทธิ์ผู้ดูแลระบบของบริษัทหรือผู้ดูแลการเรียกเก็บเงิน ถ้าคุณได้รับข้อผิดพลาดต่อไปนี้ คุณจะต้องเชื่อมต่อกับบัญชีอื่นอีกครั้ง

*ErrorMessage - เซิร์ฟเวอร์ระยะไกลส่งกลับข้อผิดพลาด: (403) Forbidden ErrorDetails - ที่ C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "ไม่สามารถลองใหม่...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : ไม่ระบุ: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

ถ้าบัญชีของคุณไม่มีสิทธิ์ผู้ดูแลระบบของบริษัทหรือผู้ดูแลการเรียกเก็บเงิน ให้ติดต่อผู้ดูแลระบบ IT ของคุณ
