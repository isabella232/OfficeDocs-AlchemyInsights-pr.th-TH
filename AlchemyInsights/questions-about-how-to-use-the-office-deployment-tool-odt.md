---
title: คำถามเกี่ยวกับวิธีการใช้เครื่องมือการปรับใช้ Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28315996"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="d6f2b-102">คำถามเกี่ยวกับวิธีการใช้เครื่องมือการปรับใช้ Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="d6f2b-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="d6f2b-103">ดาวน์โหลดเครื่องมือการปรับใช้ Office จาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](http://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="d6f2b-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="d6f2b-104">หลังจากดาวน์โหลดไฟล์ รันแบบขยายตัวเองแฟ้มปฏิบัติการ ซึ่งประกอบด้วย Office ปรับใช้เครื่องมือการเรียกใช้งานได้ (setup.exe) และแฟ้มการกำหนดค่าตัวอย่าง (configuration.xml)</span><span class="sxs-lookup"><span data-stu-id="d6f2b-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="d6f2b-105">**เมื่อต้องการแยกออก หรือเอาผลิตภัณฑ์ Office 365 ProPlus จากคอมพิวเตอร์ไคลเอนต์:**</span><span class="sxs-lookup"><span data-stu-id="d6f2b-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="d6f2b-p101">เมื่อการติดตั้ง Office 365 ProPlus คุณสามารถแยกเฉพาะผลิตภัณฑ์ เมื่อต้องการทำเช่นนี้ ให้ทำตามขั้นตอนต่าง ๆ สำหรับการติดตั้ง Office ด้วยการ ODT แต่รวมองค์ประกอบ ExcludeApp ในแฟ้มการกำหนดค่าของคุณ ตัวอย่างเช่น แฟ้มการตั้งค่าคอนฟิกนี้ติดตั้งผลิตภัณฑ์ Office 365 ProPlus ทั้งหมดยกเว้นผู้เผยแพร่:</span><span class="sxs-lookup"><span data-stu-id="d6f2b-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="d6f2b-109">ภาพรวมของเครื่องมือการปรับใช้ Office</span><span class="sxs-lookup"><span data-stu-id="d6f2b-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

