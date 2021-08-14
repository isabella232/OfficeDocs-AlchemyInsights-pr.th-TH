---
title: ข้อสงสัยเกี่ยวกับวิธีการใช้เครื่องมือการปรับใช้Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959702"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>ข้อสงสัยเกี่ยวกับวิธีการใช้เครื่องมือการปรับใช้Office (ODT)

ดาวน์โหลดOfficeการปรับใช้จาก[ศูนย์ดาวน์โหลด Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
หลังจากดาวน์โหลดไฟล์ ให้เรียกใช้ไฟล์ปฏิบัติการที่แยกตัวเอง ซึ่งมี Office Deployment Tool executable (setup.exe) และไฟล์การกําหนดค่าตัวอย่าง (configuration.xml)
  
 **เมื่อต้องการแยกหรือลบผลิตภัณฑ์Microsoft 365 Apps for enterpriseคอมพิวเตอร์ไคลเอ็นต์:**
  
เมื่อติดตั้งMicrosoft 365 Apps for enterprise คุณสามารถยกเว้นผลิตภัณฑ์เฉพาะได้ เมื่อจะติดตั้ง ให้ปฏิบัติตามขั้นตอนการติดตั้งOffice ODT แต่ให้รวมองค์ประกอบ ExcludeApp ไว้ในไฟล์การกําหนดค่าของคุณ ตัวอย่างเช่น ไฟล์การกําหนดค่านี้จะติดตั้งผลิตภัณฑ์ทั้งหมดMicrosoft 365 Apps for enterprise ยกเว้นผลิตภัณฑ์ต่อไปนี้Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[ภาพรวมของเครื่องมือOfficeผลิตภัณฑ์](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

