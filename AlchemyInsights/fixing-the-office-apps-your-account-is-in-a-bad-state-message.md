---
title: การแก้ไขแอป Microsoft 365 บัญชีของคุณอยู่ในข้อความสถานะที่ไม่ถูกต้อง
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
ms.openlocfilehash: 264307f23a349ef4ebf40f48ddbcddd3216a4927
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580136"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="6b962-102">การแก้ไขข้อผิดพลาดในแอป Microsoft 365 "บัญชีของคุณอยู่ในสถานะไม่ถูกต้อง"</span><span class="sxs-lookup"><span data-stu-id="6b962-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="6b962-103">ในการแก้ไขข้อผิดพลาดนี้ ให้ลองใช้ตัวเลือกต่อไปนี้กับคอมพิวเตอร์ที่ได้รับผลกระทบ:</span><span class="sxs-lookup"><span data-stu-id="6b962-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="6b962-104">เปิดแอป Office เลือก **ไฟล์** > **บัญชี** > **ลงชื่อออกจากบัญชีทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="6b962-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="6b962-105">ลงชื่อเข้าใช้อีกครั้งโดยใช้บัญชีผู้ใช้ที่มีสิทธิการใช้งานที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="6b962-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="6b962-106">สำหรับข้อมูลโดยละเอียด โปรดดู[บัญชีใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)</span><span class="sxs-lookup"><span data-stu-id="6b962-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="6b962-107">[ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows</span><span class="sxs-lookup"><span data-stu-id="6b962-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="6b962-108">**หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว</span><span class="sxs-lookup"><span data-stu-id="6b962-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6b962-109">ตัวอย่างเช่น \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="6b962-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="6b962-110">หากเกิดข้อผิดพลาดขณะเชื่อมต่อกับ Office 365 เมื่อใช้ Office 2013 [ให้เปิดใช้งานการรับรองความถูกต้องสมัยใหม่](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)สำหรับไคลเอ็นต์ Office</span><span class="sxs-lookup"><span data-stu-id="6b962-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="6b962-111">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[วิธีการแก้ไขปัญหาแอปที่ไม่ใช่เบราว์เซอร์ที่ไม่สามารถลงชื่อเข้าใช้ Microsoft 365, Azure หรือ Intun](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)</span><span class="sxs-lookup"><span data-stu-id="6b962-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

