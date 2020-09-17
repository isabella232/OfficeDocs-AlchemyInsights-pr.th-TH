---
title: คำถามเกี่ยวกับวิธีใช้เครื่องมือการปรับใช้ Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774910"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>คำถามเกี่ยวกับวิธีใช้เครื่องมือการปรับใช้ Office (ODT)

ดาวน์โหลดเครื่องมือการปรับใช้ Office จาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
หลังจากดาวน์โหลดไฟล์แล้วให้เรียกใช้ไฟล์ที่ปฏิบัติการได้ด้วยตนเองซึ่งมีแอปรับใช้เครื่องมือการปรับใช้ Office (setup.exe) และไฟล์การกำหนดค่าตัวอย่าง (configuration.xml)
  
 **เมื่อต้องการแยกหรือเอาแอป Microsoft ๓๖๕สำหรับผลิตภัณฑ์สำหรับองค์กรออกจากคอมพิวเตอร์ไคลเอ็นต์:**
  
เมื่อติดตั้งแอป Microsoft ๓๖๕สำหรับองค์กรคุณสามารถแยกผลิตภัณฑ์ที่เฉพาะเจาะจงได้ เมื่อต้องการทำเช่นนี้ให้ทำตามขั้นตอนสำหรับการติดตั้ง Office ด้วย ODT แต่รวมองค์ประกอบ ExcludeApp ในไฟล์การกำหนดค่าของคุณ ตัวอย่างเช่นไฟล์การกำหนดค่านี้จะติดตั้งแอป Microsoft ๓๖๕ทั้งหมดสำหรับผลิตภัณฑ์สำหรับองค์กรยกเว้น Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[ภาพรวมของเครื่องมือการปรับใช้ Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

