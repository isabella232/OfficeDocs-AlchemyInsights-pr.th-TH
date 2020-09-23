---
title: ปัญหาในการลงชื่อเข้าใช้แอป Microsoft ๓๖๕
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: a1e9844094dd164ca8bd5fb2a196161a5de0282f
ms.sourcegitcommit: 57102d7daf32f370cab84dba342819a1ad5cb261
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/23/2020
ms.locfileid: "48236144"
---
# <a name="issues-signing-into-microsoft-365-apps"></a><span data-ttu-id="2f378-102">ปัญหาในการลงชื่อเข้าใช้แอป Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="2f378-102">Issues signing into Microsoft 365 Apps</span></span>

<span data-ttu-id="2f378-103">เมื่อต้องการแก้ไขปัญหาการลงชื่อเข้าใช้ด้วยแอป Microsoft ๓๖๕ให้ลองใช้ตัวเลือกต่อไปนี้บนเครื่องจักรที่ได้รับผลกระทบ:</span><span class="sxs-lookup"><span data-stu-id="2f378-103">To fix sign-in issues with Microsoft 365 apps, try the following options on the affected machine:</span></span>  

- <span data-ttu-id="2f378-104">สำหรับ Windows ให้ดู [คำแนะนำเกี่ยวกับการแก้ไขปัญหาทั่วไปในการลงชื่อเข้าใช้](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span><span class="sxs-lookup"><span data-stu-id="2f378-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span></span>
- <span data-ttu-id="2f378-105">สำหรับ Mac ให้ดูที่  [ไม่สามารถลงชื่อเข้าใช้แอป Office ๒๐๑๖ For Mac ได้](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span><span class="sxs-lookup"><span data-stu-id="2f378-105">For Mac, see  [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span></span>

<span data-ttu-id="2f378-106">**เคล็ดลับ** บนเครื่อง Windows เราสามารถวินิจฉัยและแก้ไขปัญหาการลงชื่อเข้าใช้ Office ทั่วไปได้โดยอัตโนมัติสำหรับคุณ</span><span class="sxs-lookup"><span data-stu-id="2f378-106">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="2f378-107">ดาวน์โหลดและเรียกใช้ตัว  **[ช่วยการสนับสนุนและการกู้คืนของ Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** เพื่อใช้เครื่องมืออัตโนมัติของเรา</span><span class="sxs-lookup"><span data-stu-id="2f378-107">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="2f378-108">**หมายเหตุ:** การปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่ (ADAL) หรือการจัดการบัญชีผู้ใช้เว็บ (WAM) สำหรับการแก้ไขปัญหาการลงชื่อเข้าใช้หรือการเปิดใช้งานไม่**แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="2f378-108">**Note:** Disabling Modern Authentication (ADAL) or Web Account Management (WAM) for fixing sign-in or activation issues  **is not recommended**.</span></span> <span data-ttu-id="2f378-109">ถ้าข้อผิดพลาดเกิดขึ้นขณะเชื่อมต่อกับ Microsoft ๓๖๕โดยใช้ Office ๒๐๑๓ให้ตรวจสอบให้แน่ใจว่าคุณได้ [เปิดใช้งานการรับรองความถูกต้องที่ทันสมัย](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  สำหรับไคลเอ็นต์ Office</span><span class="sxs-lookup"><span data-stu-id="2f378-109">If the errors occur while connecting to Microsoft 365 using Office 2013, ensure that you [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  for Office client.</span></span>

<span data-ttu-id="2f378-110">สำหรับการดำเนินการแก้ไขปัญหาที่เฉพาะเจาะจงให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="2f378-110">For specific troubleshooting actions, see:</span></span>

[<span data-ttu-id="2f378-111">ปัญหาการเชื่อมต่อในการลงชื่อเข้าใช้หลังจากอัปเดตเป็น Office ๒๐๑๖รุ่น16.0.7967 บน Windows 10</span><span class="sxs-lookup"><span data-stu-id="2f378-111">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[<span data-ttu-id="2f378-112">คุณไม่สามารถลงชื่อเข้าใช้บัญชีผู้ใช้ขององค์กรของคุณเช่น Office ๓๖๕, Azure หรือ Intune</span><span class="sxs-lookup"><span data-stu-id="2f378-112">You can't sign in to your organizational account such as Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[<span data-ttu-id="2f378-113">วิธีแก้ไขปัญหาแอปที่ไม่ใช่เบราว์เซอร์ที่ไม่สามารถลงชื่อเข้าใช้ Office ๓๖๕, Azure หรือ Intune</span><span class="sxs-lookup"><span data-stu-id="2f378-113">How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune</span></span>](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[<span data-ttu-id="2f378-114">ได้รับพร้อมท์ซ้ำๆสำหรับข้อมูลประจำตัวใน Office</span><span class="sxs-lookup"><span data-stu-id="2f378-114">Repeatedly prompted for credentials in Office</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)