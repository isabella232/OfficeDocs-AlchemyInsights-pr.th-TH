---
title: ปัญหาในการลงชื่อเข้าใช้กับโปรแกรมประยุกต์ของ Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938366"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="d4da1-102">ปัญหาในการลงชื่อเข้าใช้กับโปรแกรมประยุกต์ของ Office</span><span class="sxs-lookup"><span data-stu-id="d4da1-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="d4da1-103">เมื่อต้องการแก้ไขปัญหาในการลงชื่อเข้าใช้กับโปรแกรมประยุกต์ Office ลองต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="d4da1-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="d4da1-104">เอาบัญชีงานทั้งหมด ยกเว้นบัญชีได้รับผลกระทบ โดยใช้การตั้งค่า Windows >**เข้างานหรือที่โรงเรียน**</span><span class="sxs-lookup"><span data-stu-id="d4da1-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="d4da1-105">[ข้อมูลประจำตัวของ Office ล้าง](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows</span><span class="sxs-lookup"><span data-stu-id="d4da1-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d4da1-106">**หมายเหตุ:** มีเปลี่ยนเส้นทางรีจิสทรีสำหรับ Office 2016 แปลง 16.0</span><span class="sxs-lookup"><span data-stu-id="d4da1-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d4da1-107">(แลกเปลี่ยน: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d4da1-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="d4da1-108">เปิดโปรแกรมประยุกต์ Office เลือก**แฟ้ม** > **บัญชี** > **เครื่องหมายออก** จากนั้น เข้าสู่ระบบโดยใช้บัญชีผู้ใช้ที่มีลิขสิทธิ์ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="d4da1-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="d4da1-109">สำหรับข้อมูลเพิ่มเติม ให้ดู[บัญชีผู้ใช้ใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)</span><span class="sxs-lookup"><span data-stu-id="d4da1-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="d4da1-110">สำหรับ Mac ดู[ไม่สามารถเข้าสู่ระบบเป็น 2016 Office สำหรับแอพลิเคชัน Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span><span class="sxs-lookup"><span data-stu-id="d4da1-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="d4da1-111">ถ้าข้อผิดพลาดเกิดขึ้นขณะเชื่อมต่อกับโดยใช้ Office 2013 Office 365 เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สำหรับไคลเอ็นต์ของ Office</span><span class="sxs-lookup"><span data-stu-id="d4da1-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="d4da1-112">สำหรับข้อมูลเพิ่มเติม ให้ดูที่</span><span class="sxs-lookup"><span data-stu-id="d4da1-112">For more information, see:</span></span>
- [<span data-ttu-id="d4da1-113">คุณไม่สามารถเข้าสู่ระบบ Office 365, Azure หรือ Intune</span><span class="sxs-lookup"><span data-stu-id="d4da1-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="d4da1-114">ปัญหาการเชื่อมต่อในเครื่องหลังจากการปรับปรุง Office 2016 16.0.7967 ที่สร้างบน Windows 10</span><span class="sxs-lookup"><span data-stu-id="d4da1-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="d4da1-115">"ขอโทษ บัญชีผู้ใช้อื่นจากองค์กรของคุณมีอยู่แล้วลงชื่อเข้าใช้บนคอมพิวเตอร์เครื่องนี้" ใน Office</span><span class="sxs-lookup"><span data-stu-id="d4da1-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="d4da1-116">การแก้ไขปัญหาการเข้าสู่ระบบปัญหาเกี่ยวกับการรับรองความถูกต้องแบบสมัยใหม่ของ Office เมื่อคุณใช้ ADFS</span><span class="sxs-lookup"><span data-stu-id="d4da1-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)