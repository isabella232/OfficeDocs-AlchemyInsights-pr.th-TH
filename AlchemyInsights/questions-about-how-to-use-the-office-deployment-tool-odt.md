---
title: คําถามเกี่ยวกับวิธีการใช้เครื่องมือการปรับใช้ Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698077"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>คําถามเกี่ยวกับวิธีการใช้เครื่องมือการปรับใช้ Office (ODT)

ดาวน์โหลดเครื่องมือการปรับใช้ Office จาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
หลังจากดาวน์โหลดไฟล์แล้ว ให้เรียกใช้แฟ้มที่ปฏิบัติการแยกแฟ้มด้วยตนเอง ซึ่งประกอบด้วยปฏิบัติการเครื่องมือการปรับใช้ Office (setup.exe) และแฟ้มการกําหนดค่าตัวอย่าง (configuration.xml)
  
 **เมื่อต้องการแยกหรือเอาโปรแกรมประยุกต์ Microsoft 365 สําหรับผลิตภัณฑ์ขององค์กรออกจากคอมพิวเตอร์ไคลเอนต์:**
  
เมื่อติดตั้งแอป Microsoft 365 สําหรับองค์กร คุณสามารถยกเว้นผลิตภัณฑ์ที่เฉพาะเจาะจงได้ เมื่อต้องการทําเช่นนี้ ให้ทําตามขั้นตอนสําหรับการติดตั้ง Office ด้วย ODT แต่รวมองค์ประกอบ ExcludeApp ในแฟ้มการกําหนดค่าของคุณ ตัวอย่างเช่น แฟ้มการกําหนดค่านี้ติดตั้งโปรแกรมประยุกต์ของ Microsoft 365 ทั้งหมดสําหรับผลิตภัณฑ์ขององค์กรยกเว้นผู้เผยแพร่:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[ภาพรวมของเครื่องมือการปรับใช้ Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

