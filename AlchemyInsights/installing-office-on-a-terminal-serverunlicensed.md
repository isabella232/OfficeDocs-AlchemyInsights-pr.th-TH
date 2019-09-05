---
title: การติดตั้งสำนักงานบนเซิร์ฟเวอร์เทอร์มินัล-ใบอนุญาต
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735408"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="a8249-102">การติดตั้ง Office บนเซิร์ฟเวอร์เทอร์มินัล</span><span class="sxs-lookup"><span data-stu-id="a8249-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="a8249-103">สำหรับการจัดวาง Office ๓๖๕ ProPlus บนเซิร์ฟเวอร์ Windows โดยใช้บริการเดสก์ท็อประยะไกล (RDS), เดิมชื่อบริการเทอร์มินัล:</span><span class="sxs-lookup"><span data-stu-id="a8249-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="a8249-104">คุณต้องมีแผน Office ๓๖๕ที่ประกอบด้วย Office ๓๖๕ ProPlus เช่น Office ๓๖๕เอ็นเตอร์ไพรส์ E3 หรือองค์กร E5</span><span class="sxs-lookup"><span data-stu-id="a8249-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="a8249-105">แผนพรีเมียม Office ๓๖๕ธุรกิจและ Office ๓๖๕ไม่รวม Office ๓๖๕ ProPlus</span><span class="sxs-lookup"><span data-stu-id="a8249-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="a8249-106">คุณต้องเปิดการใช้[งานคอมพิวเตอร์ที่ใช้ร่วมกัน](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="a8249-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="a8249-107">ถ้าคุณต้องการติดตั้ง Office ๓๖๕ ProPlus บน RDS จากศูนย์ดูแล Microsoft ๓๖๕***ซึ่งใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="a8249-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="a8249-108">ตรวจสอบว่าคุณมีแผน Office ๓๖๕ใดบ้าง</span><span class="sxs-lookup"><span data-stu-id="a8249-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="a8249-109">เรียนรู้วิธี</span><span class="sxs-lookup"><span data-stu-id="a8249-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="a8249-110">ถ้าจำเป็นให้สลับไปยังแผน Office ๓๖๕อื่น</span><span class="sxs-lookup"><span data-stu-id="a8249-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="a8249-111">เรียนรู้วิธี</span><span class="sxs-lookup"><span data-stu-id="a8249-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="a8249-112">ถ้า Office ถูกติดตั้งบนเซิร์ฟเวอร์ RDS โดยใช้แผน Office ๓๖๕อื่นๆที่มีอยู่ให้ถอนการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="a8249-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="a8249-113">ตัวอย่างเช่นโดยไปที่ ' แผง\>ควบคุม ' ถอนการติดตั้งโปรแกรม</span><span class="sxs-lookup"><span data-stu-id="a8249-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="a8249-114">ถอนการติดตั้งโดยใช้[ฝ่ายสนับสนุนของ Microsoft และผู้ช่วยกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)ถ้าคุณกำลังทำงานเป็นปัญหา</span><span class="sxs-lookup"><span data-stu-id="a8249-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="a8249-115">บนเซิร์ฟเวอร์ RDS ลงชื่อเข้าใช้ศูนย์ดูแลของ Microsoft ๓๖๕กับบัญชีผู้ดูแลระบบของคุณและ[ติดตั้ง Office ๓๖๕ ProPlus](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="a8249-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="a8249-116">หลังจากติดตั้ง Office แล้ว***อย่าเปิดหรือลงชื่อเข้า***ใช้โปรแกรมประยุกต์ office ใดๆ</span><span class="sxs-lookup"><span data-stu-id="a8249-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="a8249-117">บนเซิร์ฟเวอร์ RDS เปิดการใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันโดยการแก้ไขรีจิสทรีโดยทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="a8249-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="a8249-118">คลิกขวาที่ปุ่ม Windows ในมุมด้านซ้ายมือล่างของหน้าจอของคุณและเลือกเรียกใช้</span><span class="sxs-lookup"><span data-stu-id="a8249-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="a8249-119">ในกล่องเปิดพิมพ์**regedit**และจากนั้นให้เลือก ' ตกลง '</span><span class="sxs-lookup"><span data-stu-id="a8249-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="a8249-120">เลือกใช่เมื่อได้รับพร้อมท์ให้อนุญาตให้ตัวแก้ไขรีจิสทรีทำการเปลี่ยนแปลงอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="a8249-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="a8249-121">ในตัวแก้ไขรีจิสทรีเพิ่มค่าสตริงของการอนุญาตให้ใช้**สิทธิ์ Sharedคอมพิวเตอร์**ที่มีการตั้งค่าของ1ภายใต้ HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="a8249-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="a8249-122">บนเซิร์ฟเวอร์ RDS***เข้าสู่ระบบในฐานะผู้ใช้ปลาย***ทางและตรวจสอบว่าเปิดใช้งานคอมพิวเตอร์ที่ใช้[ร่วมกันสำหรับ Office ๓๖๕ ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)</span><span class="sxs-lookup"><span data-stu-id="a8249-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="a8249-123">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับข้อกำหนดเบื้องต้นคำแนะนำในการตั้งค่าและคำแนะนำเกี่ยวกับการติดตั้งแบบกำหนดเองโดยใช้เครื่องมือการปรับใช้ Office โปรดดูที่การจัดวาง[office ๓๖๕ ProPlus โดยใช้บริการเดสก์ท็อประยะไกล](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)</span><span class="sxs-lookup"><span data-stu-id="a8249-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="a8249-124">หากต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันโปรดดูที่การ[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันสำหรับ Office ๓๖๕ ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="a8249-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  