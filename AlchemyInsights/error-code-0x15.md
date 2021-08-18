---
title: รหัสข้อผิดพลาด 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งานเวอร์ชัน Office 2013 บนการปรับใช้ Remote Desktop Services (RDS) ให้พิจารณาเปิดใช้งาน ADAL โดยการแก้ไขรีจิสทรี
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316705"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>เกิดข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บน บริการเดสก์ท็อประยะไกล

ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งานเวอร์ชัน Office 2013 บนการปรับใช้ Remote Desktop Services (RDS) ให้พิจารณาเปิดใช้งาน ADAL โดยการแก้ไขรีจิสทรี
  
|**รีจิสทรีคีย์**|**ชนิด**|**ค่า**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
**หมายเหตุ**: ADAL จะถูกเปิดใช้งานตามค่าเริ่มต้นใน Microsoft 365 Apps for enterprise Office 2016 บริการเดสก์ท็อประยะไกล (RDS) เคยชื่อ Terminal Services
  