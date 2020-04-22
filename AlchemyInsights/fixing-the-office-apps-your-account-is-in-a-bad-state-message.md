---
title: การแก้ไขข้อความ บัญชีของคุณอยู่ในสถานะที่ไม่สามารถใช้งานได้ ของแอป Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: b28865ff1da434a254c9051183074be35cdd0252
ms.sourcegitcommit: 9b2b162ad651e2c3d9d0c746f67a78334592f076
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/17/2020
ms.locfileid: "43547981"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="46e13-102">การแก้ไขข้อผิดพลาด "บัญชีของคุณอยู่ในสถานะที่ไม่สามารถใช้งานได้" ของแอป Office</span><span class="sxs-lookup"><span data-stu-id="46e13-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="46e13-103">ในการแก้ไขข้อผิดพลาดนี้ ให้ลองใช้ตัวเลือกต่อไปนี้กับคอมพิวเตอร์ที่ได้รับผลกระทบ:</span><span class="sxs-lookup"><span data-stu-id="46e13-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="46e13-104">เปิดแอป Office เลือก **ไฟล์** > **บัญชี** > **ลงชื่อออกจากบัญชีทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="46e13-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="46e13-105">ลงชื่อเข้าใช้อีกครั้งโดยใช้บัญชีผู้ใช้ที่มีสิทธิการใช้งานที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="46e13-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="46e13-106">สำหรับข้อมูลโดยละเอียด โปรดดู[บัญชีใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)</span><span class="sxs-lookup"><span data-stu-id="46e13-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="46e13-107">[ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows</span><span class="sxs-lookup"><span data-stu-id="46e13-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="46e13-108">**หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว</span><span class="sxs-lookup"><span data-stu-id="46e13-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="46e13-109">ตัวอย่างเช่น \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="46e13-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="46e13-110">หากเกิดข้อผิดพลาดขณะเชื่อมต่อกับ Office 365 เมื่อใช้ Office 2013 [ให้เปิดใช้งานการรับรองความถูกต้องสมัยใหม่](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)สำหรับไคลเอ็นต์ Office</span><span class="sxs-lookup"><span data-stu-id="46e13-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="46e13-111">สำหรับข้อมูลเพิ่มเติม โปรดดู[วิธีแก้ไขปัญหาแอปที่ไม่ใช่เบราว์เซอร์ซึ่งไม่สามารถลงชื่อเข้าใช้ Office 365, Azure หรือ Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)</span><span class="sxs-lookup"><span data-stu-id="46e13-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

