---
title: การปรับใช้แอป Microsoft 365 ขององค์กรเพื่อใช้ที่แชร์บน RDS, Terminal Server หรือ VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200692"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="00f2e-102">การปรับใช้แอป Microsoft 365 ขององค์กรเพื่อใช้ที่แชร์บน RDS, Terminal Server หรือ VDI</span><span class="sxs-lookup"><span data-stu-id="00f2e-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="00f2e-103">เมื่อต้องการปรับใช้แอป Microsoft 365 For enterprise โดยใช้ Remote Desktop Services (RDS) ชื่อเดิมคือ Terminal Services ให้ทําดังนี้</span><span class="sxs-lookup"><span data-stu-id="00f2e-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="00f2e-104">คุณต้องมีแผน Microsoft 365 For Business หรือแผน Office 365 ที่มีแอป Microsoft 365 For Enterprise เช่น Office 365 Enterprise E3 หรือ Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="00f2e-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="00f2e-105">Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span><span class="sxs-lookup"><span data-stu-id="00f2e-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="00f2e-106">คุณต้องเปิดใช้งาน [การเปิดใช้งานคอมพิวเตอร์ที่](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)แชร์</span><span class="sxs-lookup"><span data-stu-id="00f2e-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="00f2e-107">คุณยังสามารถดาวน์โหลดและเรียกใช้ตัวช่วยการสนับสนุน [และการกู้คืนของ Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) เพื่อติดตั้งแอป Microsoft 365 for Enterprise ในโหมดการเปิดใช้งานคอมพิวเตอร์ที่แชร์</span><span class="sxs-lookup"><span data-stu-id="00f2e-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="00f2e-108">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อแนะนําเบื้องต้น คําแนะนําการตั้งค่า และคําแนะนําเกี่ยวกับการติดตั้งแบบปรับแต่งเองโดยใช้เครื่องมือการปรับใช้ Office ให้ดูที่ การปรับใช้แอป [Microsoft 365 สําหรับองค์กรโดยใช้บริการ](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)เดสก์ท็อประยะไกล</span><span class="sxs-lookup"><span data-stu-id="00f2e-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="00f2e-109">เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์:</span><span class="sxs-lookup"><span data-stu-id="00f2e-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="00f2e-110">ดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์กับแอป Microsoft 365 for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="00f2e-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="00f2e-111">ดู[รีเซ็ตแอป Microsoft 365 สถานะการเปิดใช้งานขององค์กร](https://go.microsoft.com/fwlink/?linkid=2109218)</span><span class="sxs-lookup"><span data-stu-id="00f2e-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="00f2e-112">ถ้าคุณต้องการติดตั้งแอป Microsoft 365 for enterprise บน RDS จากศูนย์การจัดการ Microsoft 365 ซึ่ง ***ใช้*** การตั้งค่าการติดตั้งเริ่มต้น ให้ปฏิบัติตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="00f2e-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="00f2e-113">ตรวจสอบการสมัครใช้งานที่คุณมี</span><span class="sxs-lookup"><span data-stu-id="00f2e-113">Check what subscription you have.</span></span> <span data-ttu-id="00f2e-114">[เรียนรู้วิธีการ](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="00f2e-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="00f2e-115">ถ้าจําเป็น ให้สลับไปยังการสมัครใช้งานอื่น</span><span class="sxs-lookup"><span data-stu-id="00f2e-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="00f2e-116">[เรียนรู้วิธีการ](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="00f2e-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="00f2e-117">ถ้า Office ถูกติดตั้งบนเซิร์ฟเวอร์ RDS โดยใช้การสมัครใช้งาน Microsoft อื่นๆ ให้ถอนการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="00f2e-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="00f2e-118">ตัวอย่างเช่น โดยไปที่ **แผงควบคุม**  >  **ถอนการติดตั้งโปรแกรม**</span><span class="sxs-lookup"><span data-stu-id="00f2e-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="00f2e-119">ถอนการติดตั้ง [โดยใช้ตัวช่วยการสนับสนุนและ](https://aka.ms/SARA-OfficeUninstall-Alchemy) การกู้คืนของ Microsoft ถ้าคุณพบปัญหา</span><span class="sxs-lookup"><span data-stu-id="00f2e-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="00f2e-120">บนเซิร์ฟเวอร์ RDS ให้ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft 365 ด้วยบัญชีผู้ดูแลระบบของคุณ[และติดตั้งแอป Microsoft 365 for Enterprise](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="00f2e-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="00f2e-121">หลังจากติดตั้ง Office ***แล้ว อย่าเปิดหรือลงชื่อเข้าใช้*** แอปพลิเคชัน Office ใดๆ</span><span class="sxs-lookup"><span data-stu-id="00f2e-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="00f2e-122">บนเซิร์ฟเวอร์ RDS ให้เปิดใช้งานคอมพิวเตอร์ที่แชร์โดยการแก้ไขรีจิสทรีโดยปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="00f2e-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="00f2e-123">คลิกขวาที่ปุ่ม Windows ที่มุมล่างซ้ายของหน้าจอและเลือก **เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="00f2e-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="00f2e-124">ในกล่อง เปิด ให้พิมพ์ **regedit\*\*\*\*แล้วเลือก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="00f2e-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="00f2e-125">เลือก **ใช่** เมื่อได้รับพร้อมท์ให้อนุญาตให้ Registry Editor เปลี่ยนแปลงอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="00f2e-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="00f2e-126">ใน Registry Editor ให้เพิ่มค่าสตริง **ของ SharedComputerLicensing** ด้วยการตั้งค่า 1 ภายใต้ HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="00f2e-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="00f2e-127">บนเซิร์ฟเวอร์ RDS ให้ ***ลงชื่อเข้าใช้เป็นผู้ใช้ และตรวจสอบว่าเปิดใช้งาน*** การเปิดใช้งานคอมพิวเตอร์ที่แชร์แล้ว [ในแอป Microsoft 365 For Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="00f2e-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
