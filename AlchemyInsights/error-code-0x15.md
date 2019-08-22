---
title: รหัสข้อผิดพลาด 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนการกำหนดใช้บริการเดสก์ท็อประยะไกล (RDS) พิจารณาการเปิดใช้งาน ADAL โดยการแก้ไขรีจิสทรี
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527082"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>ข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนบริการเดสก์ท็อประยะไกล

ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office 2013 บนการกำหนดใช้บริการเดสก์ท็อประยะไกล (RDS) พิจารณาการเปิดใช้งาน ADAL โดยการแก้ไขรีจิสทรี
  
|**คีย์รีจิสทรี**|**ชนิด**|**ค่า**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

สำหรับข้อมูลเพิ่มเติม ให้ดู[เปิดใช้งานการพิสูจน์ตัวจริงแบบสมัยใหม่สำหรับ 2013 Office บนอุปกรณ์ Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  ADAL ถูกเปิดใช้งาน โดยค่าเริ่มต้นใน Office 365 ProPlus และ Office 2016 บริการเดสก์ท็อประยะไกล (RDS) ก่อนหน้านี้เคยใช้ชื่อบริการเทอร์มินัล
  