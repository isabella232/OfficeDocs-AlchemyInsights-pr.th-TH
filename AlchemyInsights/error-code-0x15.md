---
title: รหัสข้อผิดพลาด 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนการปรับใช้บริการเดสก์ท็อประยะไกล (RDS) ให้ลองเปิดใช้งาน ADAL ด้วยการแก้ไขรีจิสทรี
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703157"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>ข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนบริการเดสก์ท็อประยะไกล

ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนการปรับใช้บริการเดสก์ท็อประยะไกล (RDS) ให้ลองเปิดใช้งาน ADAL ด้วยการแก้ไขรีจิสทรี
  
|**คีย์รีจิสทรี**|**ชนิด**|**ค่า**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\ซอฟต์แวร์\Microsoft\Office\15.0\ทั่วไป\ข้อมูลประจําตัว\เปิดใช้งาน  <br/> |Reg_dword  <br/> |1  <br/> |

สําหรับข้อมูลเพิ่มเติม ให้ดู[เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สําหรับ Office 2013 บนอุปกรณ์ Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  เปิดใช้งานโดยค่าเริ่มต้นในโปรแกรมประยุกต์ของ Microsoft 365 สําหรับองค์กรและ Office 2016 บริการเดสก์ท็อประยะไกล (RDS) ได้ก่อนหน้านี้ชื่อบริการเทอร์มินัล
  