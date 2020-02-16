---
title: การแก้ไขแอป Office บัญชีของคุณอยู่ในข้อความสถานะไม่ถูกต้อง
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
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969869"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="481a1-102">การแก้ไขแอปพลิเคชัน Office "บัญชีของคุณอยู่ในสถานะที่ไม่ดี"</span><span class="sxs-lookup"><span data-stu-id="481a1-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="481a1-103">เมื่อต้องการแก้ไขข้อผิดพลาดนี้ให้ลองใช้ตัวเลือกต่อไปนี้บนคอมพิวเตอร์ที่ได้รับผลกระทบ:</span><span class="sxs-lookup"><span data-stu-id="481a1-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="481a1-104">เปิดแอป Office เลือก**บัญชี** > **ไฟล์** > **ลงชื่อออกจากบัญชีทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="481a1-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="481a1-105">เข้าสู่ระบบอีกครั้งโดยใช้บัญชีผู้ใช้ที่มีใบอนุญาตที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="481a1-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="481a1-106">สำหรับข้อมูลเพิ่มเติมโปรดดู[ที่บัญชีใน Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)</span><span class="sxs-lookup"><span data-stu-id="481a1-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="481a1-107">[ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows</span><span class="sxs-lookup"><span data-stu-id="481a1-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="481a1-108">**หมายเหตุ:** เส้นทางรีจิสทรีสำหรับ Office ๒๐๑๖มีการเปลี่ยนแปลงเป็น๑๖.๐</span><span class="sxs-lookup"><span data-stu-id="481a1-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="481a1-109">ตัวอย่างเช่น \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="481a1-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="481a1-110">บนคอมพิวเตอร์ที่ได้รับผลกระทบตั้งค่า EnableADAL = 0 โดยใช้ขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="481a1-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="481a1-111">คลิกขวาที่ปุ่ม Windows และเลือก**Run**</span><span class="sxs-lookup"><span data-stu-id="481a1-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="481a1-112">ในกล่อง**เปิด**พิมพ์**Regedit**แล้วเลือก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="481a1-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="481a1-113">เลือก**ใช่**เมื่อได้รับพร้อมท์เพื่ออนุญาตให้ตัวแก้ไขรีจิสทรีเพื่อทำการเปลี่ยนแปลงไปยังอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="481a1-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="481a1-114">ในตัวแก้ไขรีจิสทรีให้เพิ่มค่า DWORD ของ EnableADAL ด้วยการตั้งค่า0ภายใต้ HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="481a1-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="481a1-115">ถ้ามีข้อผิดพลาดเกิดขึ้นขณะเชื่อมต่อกับ Office ๓๖๕ใช้ Office ๒๐๑๓[เปิดใช้งานการรับรองความถูกต้องแบบสมัยใหม่](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)สำหรับไคลเอ็นต์ของ Office</span><span class="sxs-lookup"><span data-stu-id="481a1-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="481a1-116">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่วิธีการแก้ปัญหาแอปที่ไม่ใช่เบราว์เซอร์ที่ไม่สามารถเข้าสู่ระบบ Office ๓๖๕, Azure หรือ Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)</span><span class="sxs-lookup"><span data-stu-id="481a1-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

