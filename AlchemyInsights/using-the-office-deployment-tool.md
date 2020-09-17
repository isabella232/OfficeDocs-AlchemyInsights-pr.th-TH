---
title: การใช้เครื่องมือการปรับใช้ Office
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
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794930"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="52fd7-102">การใช้เครื่องมือการปรับใช้ Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="52fd7-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="52fd7-103">คุณใช้เครื่องมือการปรับใช้ Office (ODT) เพื่อปรับใช้ office ๓๖๕เวอร์ชันของ Office</span><span class="sxs-lookup"><span data-stu-id="52fd7-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="52fd7-104">เครื่องมือการปรับใช้ Office (setup.exe) ถูกเรียกใช้จากบรรทัดคำสั่งและใช้ไฟล์ XML การกำหนดค่าเพื่อกำหนดว่าการตั้งค่าใดที่จะนำไปใช้เมื่อปรับใช้ Office</span><span class="sxs-lookup"><span data-stu-id="52fd7-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="52fd7-105">ดาวน์โหลดเครื่องมือการปรับใช้ Office เวอร์ชันล่าสุดจาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="52fd7-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="52fd7-106">ใช้ [เครื่องมือกำหนดเองของ Office (OCT)](https://config.office.com) เพื่อเลือกการกำหนดลักษณะการใช้งานของคุณและสร้างไฟล์การกำหนดค่า XML</span><span class="sxs-lookup"><span data-stu-id="52fd7-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="52fd7-107">ส่งออกไฟล์การกำหนดค่าและวางภายในโฟลเดอร์เดียวกันกับที่ setup.exe อยู่</span><span class="sxs-lookup"><span data-stu-id="52fd7-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="52fd7-108">**หมายเหตุ:** ปัญหาการติดตั้ง Office มักเกิดขึ้นเนื่องจาก misconfigured หรือไฟล์การกำหนดค่า malformatted</span><span class="sxs-lookup"><span data-stu-id="52fd7-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="52fd7-109">เมื่อต้องการหลีกเลี่ยงปัญหาดังกล่าวเราขอแนะนำให้คุณใช้เครื่องมือกำหนดเองของ Office เพื่อสร้างไฟล์การกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="52fd7-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="52fd7-110">นอกจากนี้คุณยังสามารถนำเข้าไฟล์การกำหนดค่าที่มีอยู่ลงในเครื่องมือกำหนดเองของ Office ได้อีกด้วย</span><span class="sxs-lookup"><span data-stu-id="52fd7-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="52fd7-111">จากพร้อมท์คำสั่งยกระดับให้สลับไปยังตำแหน่งที่ตั้งที่ setup.exe อยู่และเรียกใช้เครื่องมือการปรับใช้ Office ในโหมดดาวน์โหลดและระบุไฟล์การกำหนดค่าที่คุณเพิ่งบันทึก</span><span class="sxs-lookup"><span data-stu-id="52fd7-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="52fd7-112">ในตัวอย่างนี้ไฟล์การกำหนดค่าจะถูกตั้งชื่อ Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="52fd7-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setup.exe /download Configuration.xml```

<span data-ttu-id="52fd7-113">4. เรียกใช้เครื่องมือการปรับใช้ Office ในโหมดกำหนดค่าและระบุไฟล์การกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="52fd7-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setup.exe /configure Configuration.xml```

<span data-ttu-id="52fd7-114">**หมายเหตุ:** คุณต้องเรียกใช้ขั้นตอนนี้จากคอมพิวเตอร์ไคลเอ็นต์ที่คุณต้องการติดตั้ง Office และคุณต้องมีสิทธิ์ของผู้ดูแลระบบภายในบนคอมพิวเตอร์เครื่องนั้น</span><span class="sxs-lookup"><span data-stu-id="52fd7-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="52fd7-115">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการใช้เครื่องมือการปรับใช้ Office สำหรับสถานการณ์การปรับใช้ Microsoft ๓๖๕สำหรับองค์กรของคุณให้ดู[ที่ภาพรวมของเครื่องมือการปรับใช้ office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)</span><span class="sxs-lookup"><span data-stu-id="52fd7-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="52fd7-116">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับวิธีใช้เครื่องมือกำหนดเองของ Office ให้ดูที่[ภาพรวมของเครื่องมือกำหนดเองของ office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)</span><span class="sxs-lookup"><span data-stu-id="52fd7-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
