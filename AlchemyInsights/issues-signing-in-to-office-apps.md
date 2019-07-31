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
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938365"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="a0e49-102">แก้ไขข้อความ "ขออภัย บัญชีผู้ใช้อื่นจากองค์กรของคุณมีการเซ็นชื่ออยู่แล้วใน" โปรแกรมประยุกต์ของ Office</span><span class="sxs-lookup"><span data-stu-id="a0e49-102">Fixing the Office apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="a0e49-103">เมื่อต้องการแก้ไขข้อผิดพลาดนี้ ลองต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a0e49-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="a0e49-104">เอาบัญชีงานทั้งหมด ยกเว้นบัญชีได้รับผลกระทบ โดยใช้การตั้งค่า Windows >**เข้างานหรือที่โรงเรียน**</span><span class="sxs-lookup"><span data-stu-id="a0e49-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="a0e49-105">[ข้อมูลประจำตัวของ Office ล้าง](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows</span><span class="sxs-lookup"><span data-stu-id="a0e49-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="a0e49-106">**หมายเหตุ:** มีเปลี่ยนเส้นทางรีจิสทรีสำหรับ Office 2016 แปลง 16.0</span><span class="sxs-lookup"><span data-stu-id="a0e49-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a0e49-107">(แลกเปลี่ยน: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="a0e49-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="a0e49-108">เปิดโปรแกรมประยุกต์ Office เลือก**แฟ้ม** > **บัญชี** > **เครื่องหมายออก** จากนั้น เข้าสู่ระบบโดยใช้บัญชีผู้ใช้ที่มีลิขสิทธิ์ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="a0e49-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="a0e49-109">สำหรับข้อมูลเพิ่มเติม ให้ดู[บัญชีผู้ใช้ใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)</span><span class="sxs-lookup"><span data-stu-id="a0e49-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="a0e49-110">สำหรับ Mac ดู[ไม่สามารถเข้าสู่ระบบเป็น 2016 Office สำหรับแอพลิเคชัน Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span><span class="sxs-lookup"><span data-stu-id="a0e49-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="a0e49-111">สำหรับข้อมูลเพิ่มเติม ดู["ขอโทษ บัญชีผู้ใช้อื่นจากองค์กรของคุณมีอยู่แล้วลงชื่อเข้าใช้บนคอมพิวเตอร์เครื่องนี้" ใน Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="a0e49-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>