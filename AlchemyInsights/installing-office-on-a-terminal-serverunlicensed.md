---
title: การติดตั้ง office บนเทอร์มินัลเซิร์ฟเวอร์ - สิทธิ์
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919002"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="f1872-102">การติดตั้ง Office บนเทอร์มินัลเซิร์ฟเวอร์</span><span class="sxs-lookup"><span data-stu-id="f1872-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="f1872-103">สำหรับการจัดวาง ProPlus 365 Office บนเซิร์ฟเวอร์ของ Windows โดยใช้บริการเดสก์ท็อประยะไกล (RDS), เดิมคือชื่อบริการเทอร์มินัล:</span><span class="sxs-lookup"><span data-stu-id="f1872-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="f1872-p101">คุณต้องมีแผนการ Office 365 ที่มี Office 365 ProPlus เช่น E3 องค์กร 365 Office หรือองค์กร E5 แผน Office 365 ธุรกิจและค่าจ้างพิเศษธุรกิจ 365 Office ไม่มี Office 365 ProPlus</span><span class="sxs-lookup"><span data-stu-id="f1872-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="f1872-106">คุณต้องเปิดใช้งาน[คอมพิวเตอร์ที่ใช้ร่วมกัน](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="f1872-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="f1872-107">ถ้าคุณต้องการติดตั้ง Office 365 ProPlus ใน RDS จากพอร์ทัล Office 365, ***ซึ่งใช้การตั้งค่าติดตั้งเริ่มต้น***, ให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="f1872-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="f1872-p102">ตรวจสอบแผน Office 365 ใดที่คุณมี [เรียนรู้วิธี](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="f1872-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="f1872-p103">ถ้าจำเป็น การสลับไปยัง Office 365 อื่นวางแผนไว้ [เรียนรู้วิธี](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="f1872-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="f1872-p104">ถ้า Office ถูกติดตั้งบนเซิร์ฟเวอร์ RDS โดยใช้แผน Office 365 อื่น ถอนการติดตั้ง ตัวอย่างเช่น ด้วยการไปที่'แผงควบคุม'\>ถอนการติดตั้งโปรแกรม ถอนใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)ถ้าคุณกำลังใช้งานเป็นการตัดสินค้าจากคลัง</span><span class="sxs-lookup"><span data-stu-id="f1872-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="f1872-115">บนเซิร์ฟเวอร์ RDS เข้าสู่ระบบของพอร์ทัล Office 365 กับบัญชีผู้ดูแลและ[ติดตั้ง Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="f1872-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="f1872-116">หลังจากที่มีการติดตั้ง Office, ***ไม่เปิด หรือเข้าสู่ระบบ*** โปรแกรมประยุกต์ Office ใด ๆ</span><span class="sxs-lookup"><span data-stu-id="f1872-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="f1872-117">บนเซิร์ฟเวอร์ RDS เปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน โดยการแก้ไขรีจิสทรีโดยทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="f1872-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="f1872-p105">คลิกขวาปุ่มของหน้าต่างในมุมซ้ายมือด้านล่างของหน้าจอ และเลือกเรียกใช้ ในกล่องเปิด พิมพ์**regedit**และจากนั้น ให้เลือก'ตกลง'</span><span class="sxs-lookup"><span data-stu-id="f1872-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="f1872-120">เลือกใช่เมื่อได้รับพร้อมท์ให้อนุญาตให้ใช้ตัวแก้ไขรีจิสทรีเพื่อทำการเปลี่ยนแปลงไปยังอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="f1872-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="f1872-121">ใน Registry Editor เพิ่มค่าสายอักขระของ**SharedComputerLicensing**ด้วยการตั้งค่าของ 1 ภายใต้ HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="f1872-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="f1872-122">บนเซิร์ฟเวอร์ RDS, ***เข้าสู่ระบบเป็นผู้ใช้*** และ[ตรวจสอบว่า เปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันถูกเปิดใช้งาน Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)</span><span class="sxs-lookup"><span data-stu-id="f1872-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="f1872-123">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับข้อกำหนดเบื้องต้น คำแนะนำการตั้งค่า และคำแนะนำในการติดตั้งแบบกำหนดเองโดยใช้เครื่องมือการปรับใช้ Office โปรดดูที่[ปรับใช้ Office 365 ProPlus โดยใช้บริการเดสก์ท็อประยะไกล](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)</span><span class="sxs-lookup"><span data-stu-id="f1872-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="f1872-124">เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน โปรดดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสำหรับ Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="f1872-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

