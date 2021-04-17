---
title: ปัญหาในการลงชื่อเข้าใช้แอป Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 02841a1b4e92eec94fc6409941d91618f02518c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836622"
---
# <a name="issues-signing-into-microsoft-365-apps"></a><span data-ttu-id="bddb1-102">ปัญหาในการลงชื่อเข้าใช้แอป Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="bddb1-102">Issues signing into Microsoft 365 Apps</span></span>

<span data-ttu-id="bddb1-103">เมื่อต้องการแก้ไขปัญหาการลงชื่อเข้าใช้แอป Microsoft 365 ให้ลองใช้ตัวเลือกต่อไปนี้บนเครื่องที่ได้รับผลกระทบ:</span><span class="sxs-lookup"><span data-stu-id="bddb1-103">To fix sign-in issues with Microsoft 365 apps, try the following options on the affected machine:</span></span>  

- <span data-ttu-id="bddb1-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span><span class="sxs-lookup"><span data-stu-id="bddb1-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span></span>
- <span data-ttu-id="bddb1-105">For Mac,  [see Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span><span class="sxs-lookup"><span data-stu-id="bddb1-105">For Mac, see  [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span></span>

<span data-ttu-id="bddb1-106">**เคล็ดลับ** บนเครื่อง Windows เราสามารถวินิจฉัยและแก้ไขปัญหาการลงชื่อเข้าใช้ Office ทั่วไปหลายอย่างให้คุณโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="bddb1-106">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="bddb1-107">ดาวน์โหลดและเรียกใช้  **[ตัวช่วยการสนับสนุนและการกู้คืน](https://aka.ms/SaRA-OfficeSignInScenario)** ของ Microsoft เพื่อใช้เครื่องมืออัตโนมัติของเรา</span><span class="sxs-lookup"><span data-stu-id="bddb1-107">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="bddb1-108">**หมายเหตุ:** ไม่แนะให้ปิดใช้งานการรับรองความถูกต้องสมัยใหม่ (ADAL) หรือการจัดการบัญชีเว็บ (WAM) เพื่อแก้ไขปัญหาการลงชื่อเข้าใช้  **หรือ** การเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="bddb1-108">**Note:** Disabling Modern Authentication (ADAL) or Web Account Management (WAM) for fixing sign-in or activation issues  **is not recommended**.</span></span> <span data-ttu-id="bddb1-109">ถ้าเกิดข้อผิดพลาดขณะเชื่อมต่อกับ Microsoft 365 โดยใช้ Office 2013 ตรวจสอบให้แน่ใจว่าคุณเปิดใช้งาน [การรับรองความถูกต้องแบบใหม่](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  สํารับไคลเอ็นต์ Office</span><span class="sxs-lookup"><span data-stu-id="bddb1-109">If the errors occur while connecting to Microsoft 365 using Office 2013, ensure that you [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  for Office client.</span></span>

<span data-ttu-id="bddb1-110">ดูวิธีการแก้ไขปัญหาเฉพาะที่:</span><span class="sxs-lookup"><span data-stu-id="bddb1-110">For specific troubleshooting actions, see:</span></span>

[<span data-ttu-id="bddb1-111">ปัญหาการเชื่อมต่อในการลงชื่อเข้าใช้หลังจากอัปเดตเป็น Office 2016 รุ่น 16.0.7967 บน Windows 10</span><span class="sxs-lookup"><span data-stu-id="bddb1-111">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[<span data-ttu-id="bddb1-112">คุณไม่สามารถลงชื่อเข้าใช้บัญชีขององค์กรของคุณ เช่น Office 365, Azure หรือ Intuned ได้</span><span class="sxs-lookup"><span data-stu-id="bddb1-112">You can't sign in to your organizational account such as Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[<span data-ttu-id="bddb1-113">วิธีแก้ไขปัญหาแอปที่ไม่ใช่เบราว์เซอร์ที่ไม่สามารถลงชื่อเข้าใช้ Office 365, Azure หรือ Intuny</span><span class="sxs-lookup"><span data-stu-id="bddb1-113">How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune</span></span>](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[<span data-ttu-id="bddb1-114">ได้รับพร้อมท์ซ้ําๆ เกี่ยวกับข้อมูลรับรองใน Office</span><span class="sxs-lookup"><span data-stu-id="bddb1-114">Repeatedly prompted for credentials in Office</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)