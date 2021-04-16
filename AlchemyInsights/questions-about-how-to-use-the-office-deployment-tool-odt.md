---
title: ข้อสงสัยเกี่ยวกับวิธีการใช้เครื่องมือการปรับใช้ Office (ODT)
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
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790351"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="51214-102">ข้อสงสัยเกี่ยวกับวิธีการใช้เครื่องมือการปรับใช้ Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="51214-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="51214-103">ดาวน์โหลดเครื่องมือการปรับใช้ Office จาก[ศูนย์ดาวน์โหลด Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="51214-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="51214-104">หลังจากดาวน์โหลดไฟล์ ให้เรียกใช้ไฟล์ปฏิบัติการที่แยกตัวเอง ซึ่งมีไฟล์ปฏิบัติการของเครื่องมือการปรับใช้ Office (setup.exe) และไฟล์การกําหนดค่าตัวอย่าง (configuration.xml)</span><span class="sxs-lookup"><span data-stu-id="51214-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="51214-105">**เมื่อต้องการแยกหรือลบแอป Microsoft 365 ออกผลิตภัณฑ์ระดับองค์กรจากคอมพิวเตอร์ไคลเอ็นต์:**</span><span class="sxs-lookup"><span data-stu-id="51214-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="51214-106">เมื่อติดตั้งแอป Microsoft 365 ขององค์กร คุณสามารถยกเว้นผลิตภัณฑ์ที่เฉพาะเจาะจงได้</span><span class="sxs-lookup"><span data-stu-id="51214-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="51214-107">เมื่อต้องการบันทึก ให้ปฏิบัติตามขั้นตอนการติดตั้ง Office ด้วย ODT แต่ให้รวมองค์ประกอบ ExcludeApp ไว้ในไฟล์การกําหนดค่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="51214-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="51214-108">ตัวอย่างเช่น ไฟล์การกําหนดค่านี้จะติดตั้งแอป Microsoft 365 ทั้งหมดของผลิตภัณฑ์ระดับองค์กร ยกเว้น Publisher:</span><span class="sxs-lookup"><span data-stu-id="51214-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="51214-109">ภาพรวมของเครื่องมือการปรับใช้ Office</span><span class="sxs-lookup"><span data-stu-id="51214-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

