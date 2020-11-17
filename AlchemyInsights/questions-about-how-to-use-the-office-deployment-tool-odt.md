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
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086175"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="15c9e-102">คำถามเกี่ยวกับวิธีใช้เครื่องมือการปรับใช้ Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="15c9e-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="15c9e-103">ดาวน์โหลดเครื่องมือการปรับใช้ Office จาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="15c9e-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="15c9e-104">หลังจากดาวน์โหลดไฟล์แล้วให้เรียกใช้ไฟล์ที่ปฏิบัติการได้ด้วยตนเองซึ่งมีแอปรับใช้เครื่องมือการปรับใช้ Office (setupodt.exe) และไฟล์การกำหนดค่าตัวอย่าง (configuration.xml)</span><span class="sxs-lookup"><span data-stu-id="15c9e-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="15c9e-105">**เมื่อต้องการแยกหรือเอาแอป Microsoft ๓๖๕สำหรับผลิตภัณฑ์สำหรับองค์กรออกจากคอมพิวเตอร์ไคลเอ็นต์:**</span><span class="sxs-lookup"><span data-stu-id="15c9e-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="15c9e-106">เมื่อติดตั้งแอป Microsoft ๓๖๕สำหรับองค์กรคุณสามารถแยกผลิตภัณฑ์ที่เฉพาะเจาะจงได้</span><span class="sxs-lookup"><span data-stu-id="15c9e-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="15c9e-107">เมื่อต้องการทำเช่นนี้ให้ทำตามขั้นตอนสำหรับการติดตั้ง Office ด้วย ODT แต่รวมองค์ประกอบ ExcludeApp ในไฟล์การกำหนดค่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="15c9e-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="15c9e-108">ตัวอย่างเช่นไฟล์การกำหนดค่านี้จะติดตั้งแอป Microsoft ๓๖๕ทั้งหมดสำหรับผลิตภัณฑ์สำหรับองค์กรยกเว้น Publisher:</span><span class="sxs-lookup"><span data-stu-id="15c9e-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="15c9e-109">ภาพรวมของเครื่องมือการปรับใช้ Office</span><span class="sxs-lookup"><span data-stu-id="15c9e-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

