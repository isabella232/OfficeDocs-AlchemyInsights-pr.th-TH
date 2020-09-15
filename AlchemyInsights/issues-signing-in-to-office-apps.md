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
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695342"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="b7ecf-102">การแก้ไขแอป Microsoft ๓๖๕ "ขออภัยบัญชีผู้ใช้อื่นจากองค์กรของคุณได้ลงชื่อเข้าใช้แล้ว" ข้อความ</span><span class="sxs-lookup"><span data-stu-id="b7ecf-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="b7ecf-103">เมื่อต้องการแก้ไขข้อผิดพลาดนี้ให้ลองทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b7ecf-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="b7ecf-104">เอาบัญชีที่ทำงานทั้งหมดออกยกเว้นบัญชีผู้ใช้ที่ได้รับผลกระทบโดยใช้การตั้งค่า Windows >**เข้าถึงที่ทำงานหรือโรงเรียน**</span><span class="sxs-lookup"><span data-stu-id="b7ecf-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="b7ecf-105">[ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows</span><span class="sxs-lookup"><span data-stu-id="b7ecf-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="b7ecf-106">**หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว</span><span class="sxs-lookup"><span data-stu-id="b7ecf-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b7ecf-107">(เช่น: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="b7ecf-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="b7ecf-108">เปิดแอป Office เลือก**File**  >  ลงชื่อเข้าใช้**บัญชีผู้ใช้**  >  **Sign Out**ไฟล์ จากนั้นลงชื่อเข้าใช้โดยใช้บัญชีผู้ใช้ที่มีสิทธิ์การใช้งานที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="b7ecf-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="b7ecf-109">สำหรับข้อมูลโดยละเอียด โปรดดู[บัญชีใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)</span><span class="sxs-lookup"><span data-stu-id="b7ecf-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="b7ecf-110">สำหรับ Mac ให้ดูที่ [ไม่สามารถลงชื่อเข้าใช้แอป Office ๒๐๑๖ For Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)ได้</span><span class="sxs-lookup"><span data-stu-id="b7ecf-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="b7ecf-111">สำหรับข้อมูลเพิ่มเติมให้ดูที่["ขออภัยบัญชีผู้ใช้อื่นจากองค์กรของคุณได้ลงชื่อเข้าใช้บนคอมพิวเตอร์เครื่องนี้แล้ว" ใน Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="b7ecf-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>