---
title: การติดตั้ง office บนเทอร์มินัลเซิร์ฟเวอร์-สิทธิ์การใช้งาน
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663136"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="dabc9-102">การติดตั้ง Office บนเซิร์ฟเวอร์เทอร์มินัล</span><span class="sxs-lookup"><span data-stu-id="dabc9-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="dabc9-103">สำหรับการปรับใช้แอป Microsoft ๓๖๕สำหรับองค์กรบน Windows Server โดยใช้บริการเดสก์ท็อประยะไกล (RDS) ซึ่งชื่อเดิมคือบริการเทอร์มินัล:</span><span class="sxs-lookup"><span data-stu-id="dabc9-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="dabc9-104">คุณต้องมีการสมัครใช้งาน Microsoft ๓๖๕ที่มีแอป Microsoft ๓๖๕สำหรับองค์กรเช่น Office ๓๖๕ Enterprise E3 หรือ Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="dabc9-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="dabc9-105">แอป Microsoft ๓๖๕สำหรับธุรกิจและแอป Microsoft ๓๖๕สำหรับแผน business Premium ไม่รวมแอป Microsoft ๓๖๕สำหรับองค์กร</span><span class="sxs-lookup"><span data-stu-id="dabc9-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="dabc9-106">คุณจำเป็นต้องเปิดใช้งานการเปิดใช้[งานคอมพิวเตอร์ที่แชร์](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="dabc9-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="dabc9-107">ถ้าคุณต้องการติดตั้งแอป Microsoft ๓๖๕สำหรับ enterprise บน RDS จากศูนย์การจัดการ Microsoft ๓๖๕ ***ที่ใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ใช้ขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="dabc9-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="dabc9-108">นอกจากนี้คุณยังสามารถดาวน์โหลดและเรียกใช้ตัว [ช่วยการสนับสนุนและการกู้คืนของ microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) เพื่อติดตั้งแอป microsoft ๓๖๕สำหรับองค์กรในโหมดการเปิดใช้งานคอมพิวเตอร์ที่แชร์ได้</span><span class="sxs-lookup"><span data-stu-id="dabc9-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="dabc9-109">ตรวจสอบว่าคุณมีการสมัครใช้งาน Microsoft ๓๖๕อะไรบ้าง</span><span class="sxs-lookup"><span data-stu-id="dabc9-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="dabc9-110">เรียนรู้วิธี</span><span class="sxs-lookup"><span data-stu-id="dabc9-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="dabc9-111">ถ้าจำเป็นให้สลับไปยังการสมัครใช้งาน Microsoft ๓๖๕อื่น</span><span class="sxs-lookup"><span data-stu-id="dabc9-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="dabc9-112">เรียนรู้วิธี</span><span class="sxs-lookup"><span data-stu-id="dabc9-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="dabc9-113">ถ้า Office ได้รับการติดตั้งบนเซิร์ฟเวอร์ RDS แล้วโดยใช้การสมัครใช้งาน Microsoft ๓๖๕อื่นๆให้ถอนการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="dabc9-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="dabc9-114">ตัวอย่างเช่นโดยไปที่แผงควบคุม \> ถอนการติดตั้งโปรแกรม</span><span class="sxs-lookup"><span data-stu-id="dabc9-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="dabc9-115">ถอนการติดตั้งโดยใช้ตัว [ช่วยการสนับสนุนและการกู้คืนของ Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) ถ้าคุณกำลังใช้งานปัญหา</span><span class="sxs-lookup"><span data-stu-id="dabc9-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="dabc9-116">บนเซิร์ฟเวอร์ RDS ให้ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft ๓๖๕ด้วยบัญชีผู้ดูแลระบบของคุณและ[ติดตั้งแอป microsoft ๓๖๕สำหรับองค์กร](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="dabc9-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="dabc9-117">หลังจากติดตั้ง Office แล้ว ***อย่าเปิดหรือลงชื่อเข้า*** ใช้แอปพลิเคชัน office ใดๆ</span><span class="sxs-lookup"><span data-stu-id="dabc9-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="dabc9-118">บนเซิร์ฟเวอร์ RDS ให้เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่แชร์โดยการแก้ไขรีจิสทรีโดยทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="dabc9-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="dabc9-119">คลิกขวาที่ปุ่ม Windows ที่มุมล่างซ้ายของหน้าจอของคุณแล้วเลือกเรียกใช้</span><span class="sxs-lookup"><span data-stu-id="dabc9-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="dabc9-120">ในกล่องเปิดให้พิมพ์ **regedit**จากนั้นเลือกตกลง</span><span class="sxs-lookup"><span data-stu-id="dabc9-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="dabc9-121">เลือกใช่เมื่อได้รับพร้อมท์ให้อนุญาตให้แก้ไขรีจิสทรีเพื่อทำการเปลี่ยนแปลงไปยังอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="dabc9-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="dabc9-122">ใน Registry Editor ให้เพิ่มค่าสตริ **SharedComputerLicensing** ที่มีการตั้งค่า1ภายใต้ HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="dabc9-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="dabc9-123">บนเซิร์ฟเวอร์ RDS ให้***ลงชื่อเข้าใช้ในฐานะผู้ใช้***และ[ตรวจสอบว่าเปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่แชร์ไว้สำหรับแอป Microsoft ๓๖๕สำหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="dabc9-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="dabc9-124">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับข้อกำหนดเบื้องต้นการตั้งค่าคำแนะนำและคำแนะนำในการติดตั้งแบบกำหนดเองโดยใช้เครื่องมือการปรับใช้ Office โปรดดูที่[การปรับใช้แอป Microsoft ๓๖๕สำหรับองค์กรโดยใช้บริการเดสก์ท็อประยะไกล](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)</span><span class="sxs-lookup"><span data-stu-id="dabc9-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="dabc9-125">เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์โปรดดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์สำหรับแอป Microsoft ๓๖๕สำหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="dabc9-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  