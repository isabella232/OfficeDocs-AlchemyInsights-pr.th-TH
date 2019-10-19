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
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553559"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="7a577-102">คำถามเกี่ยวกับวิธีการใช้เครื่องมือการปรับใช้ Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="7a577-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="7a577-103">ดาวน์โหลดเครื่องมือการปรับใช้ Office จาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](http://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="7a577-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="7a577-104">หลังจากดาวน์โหลดแฟ้มเรียกใช้แฟ้มที่ปฏิบัติการได้ด้วยตนเองซึ่งประกอบด้วยเครื่องมือการปรับใช้ Office ที่ปฏิบัติการ (setup.exe) และแฟ้มการกำหนดค่าตัวอย่าง (การกำหนดค่า. xml)</span><span class="sxs-lookup"><span data-stu-id="7a577-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="7a577-105">**หากต้องการยกเว้นหรือเอาผลิตภัณฑ์ Office ๓๖๕ ProPlus ออกจากคอมพิวเตอร์ไคลเอนต์:**</span><span class="sxs-lookup"><span data-stu-id="7a577-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="7a577-106">เมื่อติดตั้ง Office ๓๖๕ ProPlus คุณสามารถยกเว้นผลิตภัณฑ์ที่ระบุได้</span><span class="sxs-lookup"><span data-stu-id="7a577-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="7a577-107">โดยทำตามขั้นตอนสำหรับการติดตั้ง Office ด้วย ODT แต่รวมองค์ประกอบ ExcludeApp ในไฟล์การกำหนดค่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="7a577-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="7a577-108">ตัวอย่างเช่นแฟ้มการกำหนดค่านี้จะติดตั้งผลิตภัณฑ์ Office ๓๖๕ ProPlus ทั้งหมดยกเว้นผู้เผยแพร่:</span><span class="sxs-lookup"><span data-stu-id="7a577-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="7a577-109">ภาพรวมของเครื่องมือการปรับใช้ Office</span><span class="sxs-lookup"><span data-stu-id="7a577-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

