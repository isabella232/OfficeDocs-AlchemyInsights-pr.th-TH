---
title: การปรับใช้โปรแกรมประยุกต์ 365 ของ Microsoft สําหรับองค์กรสําหรับการใช้งานที่ใช้ร่วมกันบน RDS, เซิร์ฟเวอร์เทอร์มินัล หรือ VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507605"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="3645d-102">การปรับใช้โปรแกรมประยุกต์ 365 ของ Microsoft สําหรับองค์กรสําหรับการใช้งานที่ใช้ร่วมกันบน RDS, เซิร์ฟเวอร์เทอร์มินัล หรือ VDI</span><span class="sxs-lookup"><span data-stu-id="3645d-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="3645d-103">เมื่อต้องการปรับใช้โปรแกรมประยุกต์ 365 ของ Microsoft สําหรับองค์กรโดยใช้บริการเดสก์ท็อประยะไกล (RDS), ชื่อเดิมคือบริการเทอร์มินัล:</span><span class="sxs-lookup"><span data-stu-id="3645d-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="3645d-104">คุณต้องมีแผน Microsoft 365 สําหรับธุรกิจหรือแผน Office 365 ที่มีแอป Microsoft 365 สําหรับองค์กร เช่น Office 365 Enterprise E3 หรือ Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="3645d-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="3645d-105">แอป Microsoft 365 สําหรับธุรกิจและแผนมาตรฐานพรีเมี่ยมสําหรับธุรกิจ Microsoft 365 ไม่รวมแอป Microsoft 365 สําหรับองค์กร</span><span class="sxs-lookup"><span data-stu-id="3645d-105">The Microsoft 365 Apps for business and Microsoft 365 Business Premium Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="3645d-106">คุณต้องเปิดใช้งาน[การเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="3645d-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="3645d-107">คุณยังสามารถดาวน์โหลด และเรียกใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SaRA_OfficeSCA_M365Portal)เพื่อติดตั้ง Microsoft 365 Apps สําหรับองค์กรในโหมดการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="3645d-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="3645d-108">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับข้อกําหนดเบื้องต้น[Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)</span><span class="sxs-lookup"><span data-stu-id="3645d-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="3645d-109">เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน:</span><span class="sxs-lookup"><span data-stu-id="3645d-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="3645d-110">ดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสําหรับ Microsoft 365 Apps สําหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="3645d-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="3645d-111">ดู[รีเซ็ตแอป Microsoft 365 สําหรับสถานะการเปิดใช้งานขององค์กร](https://go.microsoft.com/fwlink/?linkid=2109218)</span><span class="sxs-lookup"><span data-stu-id="3645d-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="3645d-112">ถ้าคุณต้องการติดตั้ง Microsoft 365 Apps สําหรับองค์กรบน RDS จากศูนย์การจัดการ Microsoft 365***ซึ่งใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ใช้ขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="3645d-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.    <span data-ttu-id="3645d-113">ตรวจสอบสิ่งที่คุณมีการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="3645d-113">Check what subscription you have.</span></span> <span data-ttu-id="3645d-114">[เรียนรู้วิธี](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="3645d-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.    <span data-ttu-id="3645d-115">หากจําเป็น ให้สลับไปยังการสมัครใช้งานอื่น</span><span class="sxs-lookup"><span data-stu-id="3645d-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="3645d-116">[เรียนรู้วิธี](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="3645d-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3.    <span data-ttu-id="3645d-117">ถ้า Office ถูกติดตั้งบนเซิร์ฟเวอร์ RDS โดยใช้การสมัครใช้งาน Microsoft อื่น ๆ ถอนการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="3645d-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="3645d-118">ตัวอย่างเช่น โดยไปที่**แผงควบคุม**  >  **การถอนการติดตั้งโปรแกรม**</span><span class="sxs-lookup"><span data-stu-id="3645d-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="3645d-119">ถอนการติดตั้งโดยใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)ถ้าคุณกําลังทํางานเป็นปัญหา</span><span class="sxs-lookup"><span data-stu-id="3645d-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.    <span data-ttu-id="3645d-120">บนเซิร์ฟเวอร์ RDS ให้ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft 365 ด้วยบัญชีผู้ดูแลระบบของคุณ[และติดตั้งแอป Microsoft 365 สําหรับองค์กร](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="3645d-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.    <span data-ttu-id="3645d-121">หลังจากที่มีการติดตั้ง Office***แล้ว***</span><span class="sxs-lookup"><span data-stu-id="3645d-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.    <span data-ttu-id="3645d-122">บนเซิร์ฟเวอร์ RDS เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน โดยการแก้ไขรีจิสทรี โดยทําตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="3645d-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="3645d-123">คลิกขวาที่ปุ่ม Windows ที่มุมซ้ายล่างของหน้าจอแล้วเลือก**เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="3645d-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="3645d-124">ในกล่อง เปิด ให้พิมพ์**regedit**แล้วเลือก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="3645d-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="3645d-125">เลือก**ใช่**เมื่อได้รับพร้อมท์ให้อนุญาตให้ตัวแก้ไขรีจิสทรีทําการเปลี่ยนแปลงอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="3645d-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="3645d-126">ในตัวแก้ไขรีจิสทรี ให้เพิ่มค่าสายอักขระของ**SharedComputerLicensing**ด้วยการตั้งค่า 1 ภายใต้ HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\คลิกToRun\การกําหนดค่า</span><span class="sxs-lookup"><span data-stu-id="3645d-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="3645d-127">บนเซิร์ฟเวอร์ RDS***ให้ลงชื่อเข้าใช้ในฐานะผู้ใช้ และ***[ตรวจสอบว่าเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสําหรับ Microsoft 365 Apps สําหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="3645d-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

