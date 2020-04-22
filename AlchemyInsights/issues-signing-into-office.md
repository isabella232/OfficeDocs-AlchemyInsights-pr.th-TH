---
title: ปัญหาในการลงชื่อเข้าใช้แอป Office
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763020"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="6fe35-102">ปัญหาในการลงชื่อเข้าใช้แอป Office</span><span class="sxs-lookup"><span data-stu-id="6fe35-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="6fe35-103">เมื่อต้องการแก้ไขปัญหาการลงชื่อเข้าใช้ด้วยแอป Office ให้ลองทําดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="6fe35-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="6fe35-104">ลบบัญชีที่ทํางานทั้งหมด ยกเว้นบัญชีที่ได้รับผลกระทบ โดยใช้ การตั้งค่า Windows >**การเข้าถึงงานหรือโรงเรียน**</span><span class="sxs-lookup"><span data-stu-id="6fe35-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="6fe35-105">[ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows</span><span class="sxs-lookup"><span data-stu-id="6fe35-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="6fe35-106">**หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว</span><span class="sxs-lookup"><span data-stu-id="6fe35-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6fe35-107">(เช่น: \ซอฟต์แวร์\Microsoft\Office\16.0\ทั่วไป\ข้อมูลเฉพาะตัว\)</span><span class="sxs-lookup"><span data-stu-id="6fe35-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="6fe35-108">เปิดแอป Office แล้วเลือก**ออกจากระบบบัญชี** > **Sign Out\*\*\*\*ไฟล์** >  ลงชื่อเข้าใช้ด้วยบัญชีผู้ใช้ที่มีใบอนุญาตที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="6fe35-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="6fe35-109">สำหรับข้อมูลโดยละเอียด โปรดดู[บัญชีใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)</span><span class="sxs-lookup"><span data-stu-id="6fe35-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="6fe35-110">สําหรับ Mac โปรดดูที่[ไม่สามารถลงชื่อเข้าใช้แอป Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span><span class="sxs-lookup"><span data-stu-id="6fe35-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="6fe35-111">ถ้าข้อผิดพลาดเกิดขึ้นขณะเชื่อมต่อกับ Microsoft 365 โดยใช้ Office 2013 เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่สําหรับไคลเอ็นต์ Office</span><span class="sxs-lookup"><span data-stu-id="6fe35-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="6fe35-112">สำหรับข้อมูลเพิ่มเติม ให้ดูที่</span><span class="sxs-lookup"><span data-stu-id="6fe35-112">For more information, see:</span></span>
- [<span data-ttu-id="6fe35-113">คุณไม่สามารถเข้าสู่ระบบ Microsoft 365, Azure หรือ Intune</span><span class="sxs-lookup"><span data-stu-id="6fe35-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="6fe35-114">ปัญหาการเชื่อมต่อในการเข้าสู่ระบบหลังจากการปรับปรุง Office 2016 สร้าง 16.0.7967 บน Windows 10</span><span class="sxs-lookup"><span data-stu-id="6fe35-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="6fe35-115">"ขออภัย บัญชีอื่นจากองค์กรของคุณได้ลงชื่อเข้าใช้บนคอมพิวเตอร์เครื่องนี้แล้ว" ใน Office</span><span class="sxs-lookup"><span data-stu-id="6fe35-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="6fe35-116">แก้ไขปัญหาการลงชื่อเข้าใช้ปัญหาเกี่ยวกับการรับรองความถูกต้องแบบสมัยใหม่ของ Office เมื่อคุณใช้ ADFS</span><span class="sxs-lookup"><span data-stu-id="6fe35-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)