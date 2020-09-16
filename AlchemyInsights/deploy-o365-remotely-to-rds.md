---
title: การปรับใช้แอป Microsoft ๓๖๕สำหรับองค์กรสำหรับการใช้งานร่วมกันบน RDS, Terminal Server หรือ VDI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745554"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="ca24c-102">การปรับใช้แอป Microsoft ๓๖๕สำหรับองค์กรสำหรับการใช้งานร่วมกันบน RDS, Terminal Server หรือ VDI</span><span class="sxs-lookup"><span data-stu-id="ca24c-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="ca24c-103">เมื่อต้องการปรับใช้แอป Microsoft ๓๖๕สำหรับองค์กรที่ใช้บริการเดสก์ท็อประยะไกล (RDS) ซึ่งชื่อเดิมคือบริการเทอร์มินัล:</span><span class="sxs-lookup"><span data-stu-id="ca24c-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="ca24c-104">คุณต้องมี Microsoft ๓๖๕สำหรับแผนธุรกิจหรือแผน Office ๓๖๕ที่มีแอป Microsoft ๓๖๕สำหรับองค์กรเช่น Office ๓๖๕ Enterprise E3 หรือ Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="ca24c-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="ca24c-105">แอป Microsoft ๓๖๕สำหรับธุรกิจและแผนมาตรฐานของ Microsoft ๓๖๕ Business Premium ไม่รวมแอป Microsoft ๓๖๕สำหรับองค์กร</span><span class="sxs-lookup"><span data-stu-id="ca24c-105">The Microsoft 365 Apps for business and Microsoft 365 Business Premium Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="ca24c-106">คุณต้องเปิดใช้งานการ[เปิดใช้งานคอมพิวเตอร์ที่แชร์](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="ca24c-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="ca24c-107">นอกจากนี้คุณยังสามารถดาวน์โหลดและเรียกใช้ตัว [ช่วยการสนับสนุนและการกู้คืนของ microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) เพื่อติดตั้งแอป microsoft ๓๖๕สำหรับองค์กรในโหมดการเปิดใช้งานคอมพิวเตอร์ที่แชร์ได้</span><span class="sxs-lookup"><span data-stu-id="ca24c-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="ca24c-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อกำหนดเบื้องต้นคำแนะนำการตั้งค่าและคำแนะนำเกี่ยวกับการติดตั้งแบบกำหนดเองโดยใช้เครื่องมือการปรับใช้ Office ให้ดูที่[การปรับใช้แอป Microsoft ๓๖๕สำหรับองค์กรโดยใช้บริการเดสก์ท็อประยะไกล](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)</span><span class="sxs-lookup"><span data-stu-id="ca24c-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="ca24c-109">เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์:</span><span class="sxs-lookup"><span data-stu-id="ca24c-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="ca24c-110">ดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์สำหรับแอป Microsoft ๓๖๕สำหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="ca24c-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="ca24c-111">ให้ดูที่[ตั้งค่าแอป Microsoft ๓๖๕สำหรับสถานะการเปิดใช้งานขององค์กร](https://go.microsoft.com/fwlink/?linkid=2109218)</span><span class="sxs-lookup"><span data-stu-id="ca24c-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="ca24c-112">ถ้าคุณต้องการติดตั้งแอป Microsoft ๓๖๕สำหรับ enterprise บน RDS จากศูนย์การจัดการ Microsoft ๓๖๕ ***ที่ใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ใช้ขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ca24c-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.    <span data-ttu-id="ca24c-113">ตรวจสอบว่าคุณมีการสมัครใช้งานอะไรบ้าง</span><span class="sxs-lookup"><span data-stu-id="ca24c-113">Check what subscription you have.</span></span> <span data-ttu-id="ca24c-114">[เรียนรู้วิธี](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)การ</span><span class="sxs-lookup"><span data-stu-id="ca24c-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.    <span data-ttu-id="ca24c-115">ถ้าจำเป็นให้สลับไปยังการสมัครใช้งานอื่น</span><span class="sxs-lookup"><span data-stu-id="ca24c-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="ca24c-116">[เรียนรู้วิธี](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)การ</span><span class="sxs-lookup"><span data-stu-id="ca24c-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3.    <span data-ttu-id="ca24c-117">ถ้า Office ได้รับการติดตั้งบนเซิร์ฟเวอร์ RDS แล้วโดยใช้การสมัครใช้งาน Microsoft อื่นๆให้ถอนการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="ca24c-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="ca24c-118">ตัวอย่างเช่นโดยไปที่**แผงควบคุม**  >  **ถอนการติดตั้งโปรแกรม**</span><span class="sxs-lookup"><span data-stu-id="ca24c-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="ca24c-119">ถอนการติดตั้งโดยใช้ตัว [ช่วยการสนับสนุนและการกู้คืนของ Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) ถ้าคุณกำลังใช้งานปัญหา</span><span class="sxs-lookup"><span data-stu-id="ca24c-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.    <span data-ttu-id="ca24c-120">บนเซิร์ฟเวอร์ RDS ให้ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft ๓๖๕ด้วยบัญชีผู้ดูแลระบบของคุณและ[ติดตั้งแอป microsoft ๓๖๕สำหรับองค์กร](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="ca24c-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.    <span data-ttu-id="ca24c-121">หลังจากติดตั้ง Office แล้ว ***อย่าเปิดหรือลงชื่อเข้า*** ใช้แอปพลิเคชัน office ใดๆ</span><span class="sxs-lookup"><span data-stu-id="ca24c-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.    <span data-ttu-id="ca24c-122">บนเซิร์ฟเวอร์ RDS ให้เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่แชร์โดยการแก้ไขรีจิสทรีโดยทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ca24c-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="ca24c-123">คลิกขวาที่ปุ่ม Windows ที่มุมล่างซ้ายของหน้าจอของคุณแล้วเลือก**เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="ca24c-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="ca24c-124">ในกล่องเปิดให้พิมพ์**regedit**จากนั้นเลือก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="ca24c-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="ca24c-125">เลือก **ใช่** เมื่อได้รับพร้อมท์ให้อนุญาตให้แก้ไขรีจิสทรีเพื่อทำการเปลี่ยนแปลงไปยังอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="ca24c-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="ca24c-126">ใน Registry Editor ให้เพิ่มค่าสตริ **SharedComputerLicensing** ที่มีการตั้งค่า1ภายใต้ HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="ca24c-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="ca24c-127">บนเซิร์ฟเวอร์ RDS ให้***ลงชื่อเข้าใช้ในฐานะผู้ใช้***และ[ตรวจสอบว่าเปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่แชร์ไว้สำหรับแอป Microsoft ๓๖๕สำหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="ca24c-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

