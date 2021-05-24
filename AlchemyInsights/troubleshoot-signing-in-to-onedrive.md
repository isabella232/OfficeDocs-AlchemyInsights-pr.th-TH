---
title: แก้ไขปัญหาการลงชื่อเข้าใช้OneDrive
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8283"
- "9004614"
ms.openlocfilehash: 2c9a390f38ecbba94698a352348e2e533a50ee17
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/24/2021
ms.locfileid: "52626132"
---
# <a name="troubleshoot-signing-in-to-onedrive"></a><span data-ttu-id="555b5-102">แก้ไขปัญหาการลงชื่อเข้าใช้OneDrive</span><span class="sxs-lookup"><span data-stu-id="555b5-102">Troubleshoot signing in to OneDrive</span></span>

<span data-ttu-id="555b5-103">บทความนี้จะอธิบายสถานการณ์สมมติต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="555b5-103">This article describes the following scenarios:</span></span>

- <span data-ttu-id="555b5-104">แก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้ไคลเอ็นต์OneDriveไคลเอ็นต์</span><span class="sxs-lookup"><span data-stu-id="555b5-104">Troubleshoot issues about signing in to the OneDrive sync client</span></span>
- <span data-ttu-id="555b5-105">การแก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้ไซต์ OneDrive for Business ของคุณ</span><span class="sxs-lookup"><span data-stu-id="555b5-105">Troubleshoot issues about signing in to your OneDrive for Business site</span></span>

<span data-ttu-id="555b5-106">**แก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้ไคลเอ็นต์OneDriveไคลเอ็นต์**</span><span class="sxs-lookup"><span data-stu-id="555b5-106">**Troubleshoot issues about signing in to the OneDrive sync client**</span></span>

- <span data-ttu-id="555b5-107">หากต้องการแก้ไขรหัสข้อผิดพลาด 0x004de40[ให้ดูที่ รหัสข้อผิดพลาด0x8004de40เมื่อลงชื่อเข้าใช้OneDrive](/sharepoint/troubleshoot/administration/error-0x8004de40-in-onedrive)</span><span class="sxs-lookup"><span data-stu-id="555b5-107">For steps to resolve error code 0x004de40, see [Error Code 0x8004de40 when signing in to OneDrive](/sharepoint/troubleshoot/administration/error-0x8004de40-in-onedrive).</span></span>
- <span data-ttu-id="555b5-108">ลงชื่อเข้าใช้OneDrive SharePointไซต์ของคุณโดยไปที่ไซต์ แล้วคลิกปุ่ม ซิงค์ ที่ด้านบนของแถบเมนูบนไซต์</span><span class="sxs-lookup"><span data-stu-id="555b5-108">Sign in to the OneDrive or SharePoint site by visiting the site, and click the **Sync** button in the top of the menu bar on the site.</span></span>
- <span data-ttu-id="555b5-109">ตรวจสอบให้แน่ใจว่าคุณลงชื่อเข้าใช้ในOneDrive for Business ไม่ใช่ OneDrive.com</span><span class="sxs-lookup"><span data-stu-id="555b5-109">Ensure you're signing in to OneDrive for Business, not OneDrive.com.</span></span> <span data-ttu-id="555b5-110">ถ้า URL ที่คุณเยี่ยมชมเริ่มต้นด้วย onedrive.live.com ที่ตั้งไม่ใช่สถานที่ตั้งของOneDriveธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="555b5-110">If the URL you visit starts with onedrive.live.com, that is not the location for your OneDrive for business.</span></span> <span data-ttu-id="555b5-111">วิธีง่ายๆ ในการให้แน่ใจว่าคุณลงชื่อเข้าใช้ด้วยลิงก์OneDrive for Business: แล้ว https://portal.office.com/onedrive ใช้บัญชีที่โรงเรียนหรือที่โรงเรียนเพื่อเข้าสู่ระบบ</span><span class="sxs-lookup"><span data-stu-id="555b5-111">An easy way to ensure you're signing in to OneDrive for Business is with this link: https://portal.office.com/onedrive then use your work or school account to log on.</span></span>
- <span data-ttu-id="555b5-112">หากคุณยังคงประสบปัญหา ให้พิจารณา[การรีเซ็ตOneDrive](https://support.microsoft.com/office/reset-onedrive-34701e00-bf7b-42db-b960-84905399050c)</span><span class="sxs-lookup"><span data-stu-id="555b5-112">If you're still having trouble, consider [resetting OneDrive](https://support.microsoft.com/office/reset-onedrive-34701e00-bf7b-42db-b960-84905399050c).</span></span>
- <span data-ttu-id="555b5-113">[ยกเลิกลิงก์บัญชีของคุณOneDrive](https://support.microsoft.com/office/how-to-remove-an-account-in-onedrive-72699268-9e64-45bd-b723-9a19f4512fd1)ลงชื่อเข้าใช้ไซต์ OneDrive หรือ SharePoint แล้วคลิกปุ่ม ซิงค์ ที่ด้านบนของแถบเมนูบนไซต์</span><span class="sxs-lookup"><span data-stu-id="555b5-113">[Unlink your account from OneDrive](https://support.microsoft.com/office/how-to-remove-an-account-in-onedrive-72699268-9e64-45bd-b723-9a19f4512fd1), sign in to the OneDrive or SharePoint site, and then click the **Sync** button in the top of the menu bar on the site.</span></span>

<span data-ttu-id="555b5-114">**การแก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้ไซต์ OneDrive for Business ของคุณ**</span><span class="sxs-lookup"><span data-stu-id="555b5-114">**Troubleshoot issues about signing in to your OneDrive for Business site**</span></span>

- <span data-ttu-id="555b5-115">ตรวจสอบให้แน่ใจว่าคุณลงชื่อเข้าใช้ในOneDrive for Business ไม่ใช่ OneDrive.com</span><span class="sxs-lookup"><span data-stu-id="555b5-115">Ensure you're signing into OneDrive for Business, not OneDrive.com.</span></span> <span data-ttu-id="555b5-116">ถ้า URL ที่คุณเยี่ยมชมเริ่มต้นด้วย onedrive.live.com ไม่ใช่ที่ตั้งของOneDrive for Businessของคุณ</span><span class="sxs-lookup"><span data-stu-id="555b5-116">If the URL you visit starts with onedrive.live.com, that is not the location for your OneDrive for Business.</span></span> <span data-ttu-id="555b5-117">วิธีง่ายๆ ในการให้แน่ใจว่าคุณลงชื่อเข้าใช้ด้วยลิงก์OneDrive for Business: แล้ว https://portal.office.com/onedrive ใช้บัญชีที่โรงเรียนหรือที่โรงเรียนเพื่อเข้าสู่ระบบ</span><span class="sxs-lookup"><span data-stu-id="555b5-117">An easy way to ensure you're signing in to OneDrive for Business is with this link: https://portal.office.com/onedrive then use your work or school account to log on.</span></span>
- <span data-ttu-id="555b5-118">ถ้าคุณถูกเปลี่ยนเส้นทางไปยังหน้าDelveโปรไฟล์ของคุณ ผู้ดูแลระบบ Microsoft 365จะต้องให้สิทธิ์แก่ผู้ใช้ในการสร้าง[ไซต์OneDrive for Businessของพวกเขา](https://support.microsoft.com/office/you-re-redirected-to-your-delve-profile-page-after-you-click-onedrive-on-the-microsoft-365-app-launcher-2af26640-9ddf-46c3-8912-6af30efcc7b0)</span><span class="sxs-lookup"><span data-stu-id="555b5-118">If you're redirected to your Delve profile page, a Microsoft 365 admin will need to [grant users the right to create their OneDrive for Business site](https://support.microsoft.com/office/you-re-redirected-to-your-delve-profile-page-after-you-click-onedrive-on-the-microsoft-365-app-launcher-2af26640-9ddf-46c3-8912-6af30efcc7b0).</span></span>
- <span data-ttu-id="555b5-119">ทดสอบว่าคุณสามารถเยี่ยมชมไซต์ OneDrive โดยใช้การเรียกดู[แบบ InPrivate](https://support.microsoft.com/microsoft-edge/browse-inprivate-in-microsoft-edge-e6f47704-340c-7d4f-b00d-d0cf35aa1fcc)ใน Microsoft Edge (หรือฟีเจอร์ที่คล้ายกันในเบราว์เซอร์อื่น)</span><span class="sxs-lookup"><span data-stu-id="555b5-119">Test whether you can visit the OneDrive site by using [InPrivate browsing in Microsoft Edge](https://support.microsoft.com/microsoft-edge/browse-inprivate-in-microsoft-edge-e6f47704-340c-7d4f-b00d-d0cf35aa1fcc) (or a similar feature in another browser).</span></span>
    - <span data-ttu-id="555b5-120">ถ้าการเรียกดูแบบ InPrivate ใช้งานได้ คุณอาจต้องล้างข้อมูล[การเรียกดู](https://support.microsoft.com/microsoft-edge/view-and-delete-browser-history-in-microsoft-edge-00cf7943-a9e1-975a-a33d-ac10ce454ca4)Microsoft Edgeของคุณ (หรือฟีเจอร์ที่คล้ายกันในเบราว์เซอร์อื่น)</span><span class="sxs-lookup"><span data-stu-id="555b5-120">If InPrivate browsing works, you might need to [clear your browsing data in Microsoft Edge](https://support.microsoft.com/microsoft-edge/view-and-delete-browser-history-in-microsoft-edge-00cf7943-a9e1-975a-a33d-ac10ce454ca4) (or a similar feature in another browser).</span></span>

<span data-ttu-id="555b5-121">**แก้ไขปัญหาการลงชื่อเข้าใช้Officeเพื่อซิงค์กับOneDrive**</span><span class="sxs-lookup"><span data-stu-id="555b5-121">**Troubleshoot signing into Office to sync with OneDrive**</span></span>

<span data-ttu-id="555b5-122">ถ้าคุณได้รับข้อความแสดงข้อผิดพลาด **ที่บอกว่า** อัปโหลดถูกบล็อก **ลงชื่อเข้าใช้เพื่อ** บันทึกไฟล์นี้ หรือบันทึกสําเนา คุณอาจต้องเอาสําเนาออกและเชื่อมต่อOneDrive [ใหม่Officeบริการที่เชื่อมต่อของคุณ](https://support.microsoft.com/office/how-to-resolve-upload-blocked-sign-into-save-this-file-or-save-a-copy-error-messages-32c7340c-f5fb-4ca0-a829-65d8120f81f8)</span><span class="sxs-lookup"><span data-stu-id="555b5-122">If you get an error message saying **Upload blocked**, **Sign into save this file**, or **Save a copy**, you may need to [remove and reconnect OneDrive from your Office connected services](https://support.microsoft.com/office/how-to-resolve-upload-blocked-sign-into-save-this-file-or-save-a-copy-error-messages-32c7340c-f5fb-4ca0-a829-65d8120f81f8).</span></span>

<span data-ttu-id="555b5-123">**เคล็ดลับการแก้ไขปัญหาอื่นๆ**</span><span class="sxs-lookup"><span data-stu-id="555b5-123">**Other troubleshooting tips**</span></span>

<span data-ttu-id="555b5-124">ถ้าคุณเป็นผู้ดูแลระบบส่วนกลาง สิทธิ์การใช้งาน หรือ[ผู้ใช้ ให้กําหนดสิทธิ์การใช้งานที่ถูกต้องให้กับผู้ใช้ที่ได้รับผลกระทบ](/microsoft-365/admin/manage/assign-licenses-to-users)</span><span class="sxs-lookup"><span data-stu-id="555b5-124">If you're a global, license, or user admin, [assign the correct license to the affected user](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>

