---
title: DLP อาจต้องการชนิดที่กำหนดเอง
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 872fca326065ada002300061c951620b3d9a8d0e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052920"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP อาจต้องการชนิดที่กำหนดเอง

ด้วยนโยบายการป้องกันการสูญหายของข้อมูล (DLP) คุณสามารถระบุและปกป้องข้อมูลที่สำคัญในองค์กรของคุณ ในบางสถานการณ์คุณอาจต้องสร้างชนิดข้อมูลที่ละเอียด**อ่อนของคุณเองเพื่อ**ปกป้องข้อมูลขององค์กรของคุณ

ตัวอย่างเช่นองค์กรของคุณอาจจำเป็นต้องระบุและปกป้องรหัสพนักงานหรือข้อมูลอื่นๆในรูปแบบบางอย่างที่เฉพาะเจาะจงกับองค์กรของคุณ หากเป็นเช่นนั้นให้ดูบทความต่อไปนี้สำหรับข้อมูลเพิ่มเติม
  
 **การกำหนดชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายใน**
  
ถ้าชนิดข้อมูลที่ละเอียดอ่อนในตัวจะตอบสนองความต้องการของคุณด้วยการปรับแต่งเพียงไม่กี่คุณสามารถ[กำหนดชนิดข้อมูลที่มีความละเอียดอ่อนในตัว](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)ได้ ตัวอย่างเช่นคุณสามารถเพิ่มหรือเอาคำสำคัญออกหรือเพิ่มหรือลบหลักฐานที่สนับสนุนเช่นวันที่หรือที่อยู่
  
 **การสร้างชนิดข้อมูลที่เป็นความลับที่กำหนดเอง**
  
แต่ถ้าคุณต้องการระบุและปกป้องข้อมูลที่ละเอียดอ่อนชนิดอื่นทั้งหมดคุณสามารถ[สร้างชนิดข้อมูลที่เป็นความลับแบบกำหนดเอง](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)ใน UI ของศูนย์การปฏิบัติตามกฎระเบียบ &
  
**สร้างชนิดข้อมูลที่ละเอียดอ่อนที่กำหนดเองใน PowerShell ศูนย์ปฏิบัติตามกฎระเบียบ & ความปลอดภัย**

ในที่สุดถ้า UI ไม่มีตัวเลือกทั้งหมดที่คุณต้องการคุณสามารถ[สร้างชนิดข้อมูลที่เป็นความลับที่กำหนดเองได้ในการปฏิบัติตามข้อบังคับ & PowerShell ศูนย์กลาง](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell) โดยการเริ่มต้นด้วยแฟ้ม XML คุณสามารถใช้ตัวเลือกทุกอย่างได้
