---
title: การจัดวาง Office ๓๖๕ ProPlus สำหรับใช้ร่วมกันบน RDS, เซิร์ฟเวอร์เทอร์มินัลหรือ VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959478"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="cc5f6-102">การจัดวาง Office ๓๖๕ ProPlus สำหรับใช้ร่วมกันบน RDS, เซิร์ฟเวอร์เทอร์มินัลหรือ VDI</span><span class="sxs-lookup"><span data-stu-id="cc5f6-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="cc5f6-103">เพื่อปรับใช้ Office ๓๖๕ ProPlus โดยใช้บริการเดสก์ท็อประยะไกล (RDS), เดิมชื่อบริการเทอร์มินัล:</span><span class="sxs-lookup"><span data-stu-id="cc5f6-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="cc5f6-104">คุณต้องมี Microsoft ๓๖๕สำหรับแผนธุรกิจหรือแผน Office ๓๖๕ที่รวม Office ๓๖๕ ProPlus เช่น Office ๓๖๕เอ็นเตอร์ไพรส์ E3 หรือองค์กร E5</span><span class="sxs-lookup"><span data-stu-id="cc5f6-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="cc5f6-105">แผนพรีเมียม Office ๓๖๕ธุรกิจและ Office ๓๖๕ไม่รวม Office ๓๖๕ ProPlus</span><span class="sxs-lookup"><span data-stu-id="cc5f6-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="cc5f6-106">คุณต้องเปิดการใช้[งานคอมพิวเตอร์ที่ใช้ร่วมกัน](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="cc5f6-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="cc5f6-107">นอกจากนี้คุณยังสามารถดาวน์โหลดและเรียกใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SaRA_OfficeSCA_M365Portal)เพื่อติดตั้ง Office ๓๖๕ ProPlus ในโหมดการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="cc5f6-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="cc5f6-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อกำหนดเบื้องต้นคำแนะนำในการตั้งค่าและคำแนะนำเกี่ยวกับการติดตั้งแบบกำหนดเองโดยใช้เครื่องมือการปรับใช้ Office โปรดดูที่การจัดวาง[office ๓๖๕ ProPlus โดยใช้บริการเดสก์ท็อประยะไกล](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)</span><span class="sxs-lookup"><span data-stu-id="cc5f6-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="cc5f6-109">วิธีแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน:</span><span class="sxs-lookup"><span data-stu-id="cc5f6-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="cc5f6-110">ดู[การแก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสำหรับ Office ๓๖๕ ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="cc5f6-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="cc5f6-111">ดูที่การ[ตั้งค่าสถานะการเปิดใช้งาน Office ๓๖๕ ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218)</span><span class="sxs-lookup"><span data-stu-id="cc5f6-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="cc5f6-112">ถ้าคุณต้องการติดตั้ง Office ๓๖๕ ProPlus บน RDS จากศูนย์ดูแล Microsoft ๓๖๕***ซึ่งใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ใช้ขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="cc5f6-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="cc5f6-113">ตรวจสอบว่าคุณมีแผน Office ๓๖๕ใดบ้าง</span><span class="sxs-lookup"><span data-stu-id="cc5f6-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="cc5f6-114">[เรียนรู้วิธี](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)การ</span><span class="sxs-lookup"><span data-stu-id="cc5f6-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="cc5f6-115">ถ้าจำเป็นให้สลับไปยังแผน Office ๓๖๕อื่น</span><span class="sxs-lookup"><span data-stu-id="cc5f6-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="cc5f6-116">[เรียนรู้วิธี](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)การ</span><span class="sxs-lookup"><span data-stu-id="cc5f6-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="cc5f6-117">ถ้า Office ถูกติดตั้งบนเซิร์ฟเวอร์ RDS โดยใช้แผน Office ๓๖๕อื่นๆที่มีอยู่ให้ถอนการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="cc5f6-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="cc5f6-118">ตัวอย่างเช่นโดยไปที่**แผง** > ควบคุม**ถอนการติดตั้งโปรแกรม**</span><span class="sxs-lookup"><span data-stu-id="cc5f6-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="cc5f6-119">ถอนการติดตั้งโดยใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)ถ้าคุณกำลังทำงานเป็นปัญหา</span><span class="sxs-lookup"><span data-stu-id="cc5f6-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="cc5f6-120">บนเซิร์ฟเวอร์ RDS ลงชื่อเข้าใช้ศูนย์ดูแลของ Microsoft ๓๖๕กับบัญชีผู้ดูแลระบบของคุณและ[ติดตั้ง Office ๓๖๕ ProPlus](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="cc5f6-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="cc5f6-121">หลังจากติดตั้ง Office แล้ว***อย่าเปิดหรือลงชื่อเข้า***ใช้โปรแกรมประยุกต์ office ใดๆ</span><span class="sxs-lookup"><span data-stu-id="cc5f6-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="cc5f6-122">บนเซิร์ฟเวอร์ RDS เปิดการใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันโดยการแก้ไขรีจิสทรีโดยทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="cc5f6-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="cc5f6-123">คลิกขวาที่ปุ่ม Windows ที่มุมซ้ายล่างของหน้าจอของคุณและเลือก**เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="cc5f6-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="cc5f6-124">ในกล่องเปิดพิมพ์**regedit**และจากนั้นให้เลือก **' ตกลง '**</span><span class="sxs-lookup"><span data-stu-id="cc5f6-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="cc5f6-125">เลือก**ใช่**เมื่อได้รับพร้อมท์ให้อนุญาตให้ตัวแก้ไขรีจิสทรีทำการเปลี่ยนแปลงอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="cc5f6-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="cc5f6-126">ในตัวแก้ไขรีจิสทรีเพิ่มค่าสตริงของการอนุญาตให้ใช้**สิทธิ์ Sharedคอมพิวเตอร์**ที่มีการตั้งค่าของ1ภายใต้ HKEY_LOCAL_MACHINE \ ซอฟต์แวร์ \ Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="cc5f6-127">บนเซิร์ฟเวอร์ RDS***เข้าสู่ระบบในฐานะผู้ใช้ปลาย***ทางและตรวจสอบว่าเปิดใช้งานคอมพิวเตอร์ที่ใช้[ร่วมกันสำหรับ Office ๓๖๕ ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)</span><span class="sxs-lookup"><span data-stu-id="cc5f6-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

