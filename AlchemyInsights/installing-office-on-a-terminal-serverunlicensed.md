---
title: การติดตั้งสํานักงานบนเซิร์ฟเวอร์เทอร์มินัล - ไม่มีใบอนุญาต
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763236"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="5aab1-102">การติดตั้ง Office บนเซิร์ฟเวอร์เทอร์มินัล</span><span class="sxs-lookup"><span data-stu-id="5aab1-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="5aab1-103">สําหรับการปรับใช้โปรแกรมประยุกต์ของ Microsoft 365 สําหรับองค์กรบนเซิร์ฟเวอร์ Windows โดยใช้บริการเดสก์ท็อประยะไกล (RDS), เดิมชื่อบริการเทอร์มินัล:</span><span class="sxs-lookup"><span data-stu-id="5aab1-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="5aab1-104">คุณต้องมีการสมัครใช้งาน Microsoft 365 ที่มีแอป Microsoft 365 สําหรับองค์กร เช่น Office 365 Enterprise E3 หรือ E5 สําหรับองค์กร</span><span class="sxs-lookup"><span data-stu-id="5aab1-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="5aab1-105">แอป Microsoft 365 สําหรับธุรกิจและแอป Microsoft 365 สําหรับธุรกิจแบบพรีเมียมไม่มีแอป Microsoft 365 สําหรับองค์กร</span><span class="sxs-lookup"><span data-stu-id="5aab1-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="5aab1-106">คุณต้องเปิดใช้งาน[การเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="5aab1-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="5aab1-107">ถ้าคุณต้องการติดตั้งแอป Microsoft 365 สําหรับองค์กรบน RDS จากศูนย์การจัดการ Microsoft 365***ซึ่งใช้การตั้งค่าการติดตั้งเริ่มต้น***ให้ใช้ขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="5aab1-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="5aab1-108">คุณยังสามารถดาวน์โหลด และเรียกใช้[การสนับสนุนของ Microsoft และผู้ช่วยการกู้คืน](https://aka.ms/SaRA_OfficeSCA_M365Portal)การติดตั้ง Microsoft 365 Apps สําหรับองค์กรในโหมดการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="5aab1-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="5aab1-109">ตรวจสอบการสมัครใช้งาน Microsoft 365 ที่คุณมี</span><span class="sxs-lookup"><span data-stu-id="5aab1-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="5aab1-110">เรียนรู้วิธีการ</span><span class="sxs-lookup"><span data-stu-id="5aab1-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="5aab1-111">ถ้าจําเป็น ให้สลับไปยังการสมัครใช้งาน Microsoft 365 อื่น</span><span class="sxs-lookup"><span data-stu-id="5aab1-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="5aab1-112">เรียนรู้วิธีการ</span><span class="sxs-lookup"><span data-stu-id="5aab1-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="5aab1-113">ถ้า Office ได้รับการติดตั้งไว้แล้วบนเซิร์ฟเวอร์ RDS โดยใช้การสมัครใช้งาน Microsoft 365 อื่นๆ ให้ถอนการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="5aab1-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="5aab1-114">ตัวอย่างเช่น โดยไปที่แผงควบคุม\>ถอนการติดตั้งโปรแกรม</span><span class="sxs-lookup"><span data-stu-id="5aab1-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="5aab1-115">ถอนการติดตั้งโดยใช้[การสนับสนุนของ Microsoft และผู้ช่วยการกู้คืน](https://aka.ms/SARA-OfficeUninstall-Alchemy)ถ้าคุณกําลังพบปัญหา</span><span class="sxs-lookup"><span data-stu-id="5aab1-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="5aab1-116">บนเซิร์ฟเวอร์ RDS ลงชื่อเข้าใช้ศูนย์การจัดการ Microsoft 365 ด้วยบัญชีผู้ดูแลระบบของคุณ[และติดตั้ง Microsoft 365 Apps สําหรับองค์กร](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="5aab1-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="5aab1-117">หลังจากที่ติดตั้ง Office***don't open or sign in***แล้ว</span><span class="sxs-lookup"><span data-stu-id="5aab1-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="5aab1-118">บนเซิร์ฟเวอร์ RDS เปิดใช้งานการเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกัน โดยการแก้ไขรีจิสทรี โดยทําตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="5aab1-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="5aab1-119">คลิกขวาที่ปุ่ม Windows ที่มุมล่างซ้ายของหน้าจอและเลือก</span><span class="sxs-lookup"><span data-stu-id="5aab1-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="5aab1-120">ในกล่อง เปิด ให้พิมพ์**regedit**แล้วเลือก ตกลง</span><span class="sxs-lookup"><span data-stu-id="5aab1-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="5aab1-121">เลือก ใช่ เมื่อได้รับพร้อมท์เพื่ออนุญาตให้ตัวแก้ไขรีจิสทรีทําการเปลี่ยนแปลงอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="5aab1-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="5aab1-122">ในตัวแก้ไขรีจิสทรี เพิ่มค่าสายอักขระของ**SharedComputerLicensing**ด้วยการตั้งค่า 1 ภายใต้HKEY_LOCAL_MACHINE\ซอฟต์แวร์\Microsoft \คลิกเรียกใช้\การกําหนดค่า.</span><span class="sxs-lookup"><span data-stu-id="5aab1-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="5aab1-123">บนเซิร์ฟเวอร์ RDS***เข้าสู่ระบบในฐานะผู้ใช้***และ[ตรวจสอบว่า การเปิดใช้งานคอมพิวเตอร์ที่ใช้ร่วมกันถูกเปิดใช้งานสําหรับ Microsoft 365 Apps สําหรับองค์กร](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)</span><span class="sxs-lookup"><span data-stu-id="5aab1-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="5aab1-124">สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับข้อกําหนดเบื้องต้น[Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)</span><span class="sxs-lookup"><span data-stu-id="5aab1-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="5aab1-125">เมื่อต้องการแก้ไขข้อผิดพลาดที่เกี่ยวข้องกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์ โปรดดู[แก้ไขปัญหาเกี่ยวกับการเปิดใช้งานคอมพิวเตอร์ที่แชร์สําหรับ Microsoft 365 Apps for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="5aab1-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  