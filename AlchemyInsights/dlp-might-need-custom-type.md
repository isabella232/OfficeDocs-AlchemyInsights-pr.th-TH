---
title: DLP อาจจำเป็นต้องเป็นชนิดกำหนดเอง
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 8b49afcf50e5eb53f517bbdbd002fb80dddb6f9b
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389704"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP อาจจำเป็นต้องเป็นชนิดกำหนดเอง

นโยบาย (DLP) การป้องกันข้อมูลสูญหาย คุณสามารถระบุ และป้องกันข้อมูลที่สำคัญในองค์กรของคุณ ในบางสถานการณ์ คุณอาจต้องการสร้างชนิดข้อมูลที่เป็นความลับของผู้ใช้**แบบกำหนดเอง**เพื่อปกป้องข้อมูลขององค์กรของคุณ

ตัวอย่างเช่น ที่องค์กรของคุณอาจจำเป็นต้องระบุ และป้องกันรหัสพนักงานหรือข้อมูลอื่น ๆ ในบางรูปแบบเฉพาะในชื่อของคุณ ถ้าเป็นเช่นนั้น ดูบทความต่อไปนี้สำหรับข้อมูลเพิ่มเติม
  
 **กำหนดชนิดข้อมูลที่สำคัญอยู่แล้วภายใน**
  
ถ้าชนิดข้อมูลที่สำคัญอยู่แล้วภายในจะต้องตรงกับความต้องการของคุณ มีเพียงไม่กี่ tweaks คุณสามารถ[กำหนดชนิดข้อมูลที่สำคัญอยู่แล้วภายใน](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type) ตัวอย่างเช่น คุณสามารถเพิ่ม หรือเอาคำสำคัญ หรือเพิ่ม หรือเอาหลักฐานที่สนับสนุนเช่นวันหรือที่อยู่
  
 **สร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญ**
  
แต่ถ้าคุณจำเป็นต้องระบุ และปกป้องข้อมูลสำคัญชนิดอื่นทั้งหมด คุณสามารถ[สร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญ](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)ใน UI ของ & ความปลอดภัยศูนย์การปฏิบัติตามกฎระเบียบ
  
**สร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญในการรักษาความปลอดภัย & PowerShell ศูนย์ปฏิบัติตามกฎระเบียบ**

ในตอนท้าย ถ้า UI ไม่ได้จัดเตรียมตัวเลือกทั้งหมดที่คุณจำเป็น คุณสามารถ[สร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญในการรักษาความปลอดภัย & PowerShell ศูนย์ปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell) โดยเริ่มต้นด้วยแฟ้ม XML คุณสามารถใช้ตัวเลือกทุกตัวพร้อมใช้งาน
