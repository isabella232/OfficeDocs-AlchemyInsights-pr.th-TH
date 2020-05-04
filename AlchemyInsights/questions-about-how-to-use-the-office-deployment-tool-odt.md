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
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010777"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="4bd8e-102">คําถามเกี่ยวกับวิธีการใช้เครื่องมือการปรับใช้ Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="4bd8e-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="4bd8e-103">ดาวน์โหลดเครื่องมือการปรับใช้ Office จาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="4bd8e-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="4bd8e-104">หลังจากดาวน์โหลดไฟล์แล้ว ให้เรียกใช้แฟ้มที่ปฏิบัติการแยกแฟ้มด้วยตนเอง ซึ่งประกอบด้วยปฏิบัติการเครื่องมือการปรับใช้ Office (setup.exe) และแฟ้มการกําหนดค่าตัวอย่าง (configuration.xml)</span><span class="sxs-lookup"><span data-stu-id="4bd8e-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="4bd8e-105">**เมื่อต้องการแยกหรือเอาโปรแกรมประยุกต์ Microsoft 365 สําหรับผลิตภัณฑ์ขององค์กรออกจากคอมพิวเตอร์ไคลเอนต์:**</span><span class="sxs-lookup"><span data-stu-id="4bd8e-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="4bd8e-106">เมื่อติดตั้งแอป Microsoft 365 สําหรับองค์กร คุณสามารถยกเว้นผลิตภัณฑ์ที่เฉพาะเจาะจงได้</span><span class="sxs-lookup"><span data-stu-id="4bd8e-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="4bd8e-107">เมื่อต้องการทําเช่นนี้ ให้ทําตามขั้นตอนสําหรับการติดตั้ง Office ด้วย ODT แต่รวมองค์ประกอบ ExcludeApp ในแฟ้มการกําหนดค่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="4bd8e-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="4bd8e-108">ตัวอย่างเช่น แฟ้มการกําหนดค่านี้ติดตั้งโปรแกรมประยุกต์ของ Microsoft 365 ทั้งหมดสําหรับผลิตภัณฑ์ขององค์กรยกเว้นผู้เผยแพร่:</span><span class="sxs-lookup"><span data-stu-id="4bd8e-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="4bd8e-109">ภาพรวมของเครื่องมือการปรับใช้ Office</span><span class="sxs-lookup"><span data-stu-id="4bd8e-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

