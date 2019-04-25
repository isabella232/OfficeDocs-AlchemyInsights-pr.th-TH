---
title: คำถามเกี่ยวกับวิธีการใช้เครื่องมือการปรับใช้ Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371787"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>คำถามเกี่ยวกับวิธีการใช้เครื่องมือการปรับใช้ Office (ODT)

ดาวน์โหลดเครื่องมือการปรับใช้ Office จาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](http://go.microsoft.com/fwlink/p/?LinkID=626065)
  
หลังจากดาวน์โหลดไฟล์ รันแบบขยายตัวเองแฟ้มปฏิบัติการ ซึ่งประกอบด้วย Office ปรับใช้เครื่องมือการเรียกใช้งานได้ (setup.exe) และแฟ้มการกำหนดค่าตัวอย่าง (configuration.xml)
  
 **เมื่อต้องการแยกออก หรือเอาผลิตภัณฑ์ Office 365 ProPlus จากคอมพิวเตอร์ไคลเอนต์:**
  
เมื่อการติดตั้ง Office 365 ProPlus คุณสามารถแยกเฉพาะผลิตภัณฑ์ เมื่อต้องการทำเช่นนี้ ให้ทำตามขั้นตอนต่าง ๆ สำหรับการติดตั้ง Office ด้วยการ ODT แต่รวมองค์ประกอบ ExcludeApp ในแฟ้มการกำหนดค่าของคุณ ตัวอย่างเช่น แฟ้มการตั้งค่าคอนฟิกนี้ติดตั้งผลิตภัณฑ์ Office 365 ProPlus ทั้งหมดยกเว้นผู้เผยแพร่:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[ภาพรวมของเครื่องมือการปรับใช้ Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

