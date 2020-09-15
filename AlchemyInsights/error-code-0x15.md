---
title: รหัสข้อผิดพลาด0x15
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
description: ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office ๒๐๑๓บนการปรับใช้บริการเดสก์ท็อประยะไกล (RDS) ให้ลองเปิดใช้งานการ ADAL โดยการแก้ไขรีจิสทรี
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709206"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>เกิดข้อผิดพลาดขณะเปิดใช้งาน Office ๒๐๑๓บนบริการเดสก์ท็อประยะไกล

ถ้าคุณได้รับข้อผิดพลาดขณะเปิดใช้งาน Office ๒๐๑๓บนการปรับใช้บริการเดสก์ท็อประยะไกล (RDS) ให้ลองเปิดใช้งานการ ADAL โดยการแก้ไขรีจิสทรี
  
|**รีจิสทรีคีย์**|**ชนิด**|**ค่า**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

สำหรับข้อมูลเพิ่มเติมให้ดู[ที่เปิดใช้งานการรับรองความถูกต้องที่ทันสมัยสำหรับ Office ๒๐๑๓บนอุปกรณ์ Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  ADAL จะถูกเปิดใช้งานตามค่าเริ่มต้นในแอป Microsoft ๓๖๕สำหรับองค์กรและ Office ๒๐๑๖ บริการเดสก์ท็อประยะไกล (RDS) ถูกชื่อว่าบริการเทอร์มินัลก่อนหน้านี้
  