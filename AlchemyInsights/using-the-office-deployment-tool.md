---
title: การใช้เครื่องมือOfficeเครื่องมือการปรับใช้
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083789"
---
# <a name="using-the-office-deployment-tool-odt"></a>การใช้เครื่องมือOfficeการปรับใช้ (ODT)

คุณใช้เครื่องมือOfficeการปรับใช้ (ODT) ในการปรับใช้Office 365เวอร์ชันOffice The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.
  
1. ดาวน์โหลดเครื่องมือการปรับใช้งานOfficeเวอร์ชันล่าสุดจาก[ศูนย์ดาวน์โหลด Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. ส่งออกไฟล์การกําหนดค่าและวางไว้ในโฟลเดอร์เดียวกันsetup.exeอยู่

    **หมายเหตุ:** Officeการติดตั้งใหม่มักเกิดขึ้นเนื่องจากไฟล์การกําหนดค่าที่ผิดพลาดหรือรูปแบบผิดปกติ เมื่อต้องการหลีกเลี่ยงปัญหาดังกล่าว เราขอแนะOfficeเครื่องมือการกําหนดค่าเพื่อสร้างไฟล์การกําหนดค่า คุณยังสามารถนําเข้าไฟล์การกําหนดค่าที่มีอยู่ลงในเครื่องมือการกําหนดOfficeเองได้

3. จากพร้อมท์ของสั่งด้วยสิทธิ์ผู้ดูแล ให้สลับไปยังsetup.exeที่ตั้งที่คุณอยู่ และเรียกใช้เครื่องมือการปรับใช้ Office ในโหมดดาวน์โหลด และระบุไฟล์การกําหนดค่าที่คุณเพิ่งบันทึก ในตัวอย่างนี้ ไฟล์การกําหนดค่าจะถูกตั้งชื่อConfiguration.xml:

```setup.exe /download Configuration.xml```

4.เรียกใช้เครื่องมือOfficeการปรับใช้งานในโหมดกําหนดค่าและระบุไฟล์การกําหนดค่า

```setup.exe /configure Configuration.xml```

**หมายเหตุ:** คุณต้องเรียกใช้ขั้นตอนนี้จากคอมพิวเตอร์ไคลเอ็นต์ที่คุณต้องการติดตั้งไคลเอ็นต์และOfficeสิทธิ์ระดับผู้ดูแลระบบภายในเครื่องบนคอมพิวเตอร์เครื่องนั้น

เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการใช้ Officeเครื่องมือการปรับใช้งานMicrosoft 365 Apps for enterpriseสถานการณ์การปรับใช้ ให้ดูที่[ภาพรวมของเครื่องมือOfficeการปรับใช้](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
