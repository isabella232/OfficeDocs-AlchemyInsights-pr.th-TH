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
description: ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนการปรับใช้บริการเดสก์ท็อประยะไกล (RDS) ให้พิจารณาการเปิดใช้งาน ADAL โดยการแก้ไขรีจิสทรี
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506865"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>ข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนบริการเดสก์ท็อประยะไกล

ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนการปรับใช้บริการเดสก์ท็อประยะไกล (RDS) ให้พิจารณาการเปิดใช้งาน ADAL โดยการแก้ไขรีจิสทรี
  
|**คีย์รีจิสทรี**|**ชนิด**|**ค่า**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\ซอฟต์แวร์\Microsoft\Office\15.0\ทั่วไป\รหัสประจําตัว\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การเปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สําหรับ Office 2013 บนอุปกรณ์ Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  ADAL ถูกเปิดใช้งานโดยค่าเริ่มต้นใน Microsoft 365 Apps สําหรับองค์กรและ Office 2016 บริการเดสก์ท็อประยะไกล (RDS) ถูกตั้งชื่อก่อนหน้านี้บริการเทอร์มินัล
  