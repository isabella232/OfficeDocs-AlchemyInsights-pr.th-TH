---
title: ปัญหาเกี่ยวกับข้อมูลรับรอง
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063721"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="59fbf-102">ปัญหาเกี่ยวกับข้อมูลรับรอง</span><span class="sxs-lookup"><span data-stu-id="59fbf-102">Issues with credentials</span></span>

<span data-ttu-id="59fbf-103">[แพลตฟอร์มข้อมูลเฉพาะตัวของไมโครซอฟท์และข้อมูลเฉพาะตัวของไคลเอ็นต์ OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) จะอธิบายวิธีการโปรแกรมโดยตรงกับโฟลว์การให้ข้อมูลเฉพาะตัวของไคลเอ็นต์ OAuth 2.0</span><span class="sxs-lookup"><span data-stu-id="59fbf-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="59fbf-104">**ฉันจะจัดการรหัสผ่านหรือข้อมูลรับรองความถูกต้องของแอปพลิเคชันได้อย่างไร**</span><span class="sxs-lookup"><span data-stu-id="59fbf-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="59fbf-105">ใน Azure CLI คุณสามารถใช้ข้อมูลรับรอง [ของแอป Az](https://docs.microsoft.com/cli/azure/ad/app/credential) เพื่อลบ รายการ หรือรีเซ็ตรหัสผ่านหรือข้อมูลรับรองใบรับรองของแอปพลิเคชันได้</span><span class="sxs-lookup"><span data-stu-id="59fbf-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="59fbf-106">**ผู้ใช้ของฉันจะตั้งค่ารหัสผ่านของพวกเขาใหม่ได้อย่างไร**</span><span class="sxs-lookup"><span data-stu-id="59fbf-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="59fbf-107">ผู้ใช้ต้อง [ลงทะเบียนรีเซ็ตรหัสผ่านด้วยตนเองก่อน](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) จึงจะสามารถรีเซ็ตรหัสผ่านของพวกเขาได้</span><span class="sxs-lookup"><span data-stu-id="59fbf-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="59fbf-108">เมื่อผู้ใช้ลงทะเบียนแล้ว พวกเขาสามารถปฏิบัติตามคําแนะนําในบทความนี้เพื่อตั้งค่ารหัสผ่านของพวกเขาใหม่: [รีเซ็ตรหัสผ่านที่โรงเรียนหรือที่โรงเรียน](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)ของคุณ</span><span class="sxs-lookup"><span data-stu-id="59fbf-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="59fbf-109">**ผู้ใช้ของฉันเปลี่ยนรหัสผ่านได้อย่างไร**</span><span class="sxs-lookup"><span data-stu-id="59fbf-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="59fbf-110">ผู้ใช้สามารถปฏิบัติตามขั้นตอนในบทความนี้เพื่อเปลี่ยนรหัสผ่านของพวกเขา: [วิธีเปลี่ยนรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)ของคุณ</span><span class="sxs-lookup"><span data-stu-id="59fbf-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="59fbf-111">นอกจากนี้ พวกเขา [ยังสามารถจัดการรหัสผ่านแอปเพื่อการตรวจสอบสอง](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)ขั้นตอน</span><span class="sxs-lookup"><span data-stu-id="59fbf-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="59fbf-112">**ผู้ใช้ของฉันได้รับข้อผิดพลาดเมื่อเปลี่ยนแปลงหรือรีเซ็ตรหัสผ่านของพวกเขา**</span><span class="sxs-lookup"><span data-stu-id="59fbf-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="59fbf-113">ลิงก์นี้จะให้ข้อมูลเกี่ยวกับปัญหาทั่วไปที่อาจเกิดขึ้นเมื่อผู้ใช้พยายามรีเซ็ตรหัสผ่าน: [ปัญหาทั่วไปและวิธีแก้ไขปัญหา](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="59fbf-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="59fbf-114">**ฉันพบปัญหาในการตั้งค่ารหัสผ่านของผู้ใช้ใหม่**</span><span class="sxs-lookup"><span data-stu-id="59fbf-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="59fbf-115">ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้รีเซ็ตรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="59fbf-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="59fbf-116">*เฉพาะผู้ดูแลระบบส่วนกลาง รหัสผ่าน และผู้ดูแลระบบของผู้ใช้เท่านั้นที่สามารถตั้งค่ารหัสผ่านของผู้ใช้ใหม่ได้*</span><span class="sxs-lookup"><span data-stu-id="59fbf-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="59fbf-117">ผู้ดูแลระบบส่วนกลางยังสามารถตั้งค่ารหัสผ่านของผู้ดูแลระบบที่มีสิทธิ์ใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="59fbf-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="59fbf-118">ตรวจสอบให้แน่ใจว่าคุณเข้าใจความต้องการด้านสิทธิ์การใช้งาน:</span><span class="sxs-lookup"><span data-stu-id="59fbf-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="59fbf-119">คุณต้องได้รับมอบหมายสิทธิ์การใช้งานอย่างน้อยหนึ่งสิทธิ์ในองค์กรของคุณ ดังนี้</span><span class="sxs-lookup"><span data-stu-id="59fbf-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="59fbf-120">**ระบบคลาวด์เฉพาะผู้ใช้** - Office 365 (O365) ชําระเงิน SKU หรือ Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="59fbf-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="59fbf-121">**ผู้ใช้ระบบคลาวด์และ/หรือผู้ใช้ในองค์กร** - Azure AD Premium P1 หรือ P2, Enterprise Mobility + Security (EMS) หรือ Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="59fbf-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="59fbf-122">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับข้อความต้องการของสิทธิ์การใช้งาน ให้ดู[ข้อกฎหมายการให้สิทธิ์การใช้งานรีเซ็ตรหัสผ่านด้วยตนเองของ Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="59fbf-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="59fbf-123">เมื่อต้องการรีเซ็ตรหัสผ่านของผู้ใช้ ให้ค้นหาผู้ใช้ใน Azure AD</span><span class="sxs-lookup"><span data-stu-id="59fbf-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="59fbf-124">จากนั้น บนใบภาพรวมของผู้ใช้นั้น ให้คลิกปุ่ม "รีเซ็ตรหัสผ่าน"</span><span class="sxs-lookup"><span data-stu-id="59fbf-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="59fbf-125">**ปุ่มรีเซ็ตรหัสผ่านเป็นสีเทา**</span><span class="sxs-lookup"><span data-stu-id="59fbf-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="59fbf-126">คุณไม่ได้รับอนุญาตให้ **รีเซ็ต** รหัสผ่านของผู้ใช้นี้</span><span class="sxs-lookup"><span data-stu-id="59fbf-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="59fbf-127">*เฉพาะผู้ดูแลระบบส่วนกลาง รหัสผ่าน และผู้ดูแลระบบของผู้ใช้เท่านั้นที่สามารถตั้งค่ารหัสผ่านผู้ใช้ใหม่ได้*</span><span class="sxs-lookup"><span data-stu-id="59fbf-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="59fbf-128">ผู้ดูแลระบบส่วนกลางยังสามารถตั้งค่ารหัสผ่านของผู้ดูแลระบบที่มีสิทธิ์ใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="59fbf-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="59fbf-129">**ฉันไม่เห็นใบรีเซ็ตรหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="59fbf-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="59fbf-130">คุณไม่ได้รับอนุญาตให้ตั้งค่ารหัสผ่านใหม่</span><span class="sxs-lookup"><span data-stu-id="59fbf-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="59fbf-131">*เฉพาะผู้ดูแลระบบส่วนกลาง รหัสผ่าน และผู้ดูแลระบบของผู้ใช้เท่านั้นที่สามารถตั้งค่ารหัสผ่านผู้ใช้ใหม่ได้*</span><span class="sxs-lookup"><span data-stu-id="59fbf-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="59fbf-132">ผู้ดูแลระบบส่วนกลางยังสามารถตั้งค่ารหัสผ่านของผู้ดูแลระบบที่มีสิทธิ์ใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="59fbf-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="59fbf-133">**ฉันไม่เห็นใบผสานภายในองค์กรในการรีเซ็ตรหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="59fbf-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="59fbf-134">ใบผสานภายในองค์กรจะปรากฏเฉพาะในสภาพแวดล้อมแบบไฮบริดเท่านั้น หมายความว่าคุณใช้ Writeback ของรหัสผ่านเพื่อจัดการรหัสผ่านของผู้ใช้ภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="59fbf-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="59fbf-135">คุณไม่เห็นใบนี้หาก:</span><span class="sxs-lookup"><span data-stu-id="59fbf-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="59fbf-136">คุณไม่ได้ใช้ Writeback รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="59fbf-136">You are not using password writeback</span></span>
  - <span data-ttu-id="59fbf-137">มีปัญหากับการติดตั้ง/การเชื่อมต่อของ Writeback รหัสผ่านของคุณ</span><span class="sxs-lookup"><span data-stu-id="59fbf-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="59fbf-138">มีปัญหากับการติดตั้ง/การเชื่อมต่อของ Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="59fbf-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="59fbf-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="59fbf-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="59fbf-140">**ฉันไม่รู้วิธีรีเซ็ตรหัสผ่านของผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="59fbf-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="59fbf-141">ลงชื่อเข้าใช้พอร์ทัล Azure ในฐานะผู้ดูแลระบบที่เหมาะสม</span><span class="sxs-lookup"><span data-stu-id="59fbf-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="59fbf-142">ไปที่ Blade **ผู้ใช้และ** กลุ่ม **เลือก ผู้ใช้** ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="59fbf-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="59fbf-143">เลือกผู้ใช้จากรายการ</span><span class="sxs-lookup"><span data-stu-id="59fbf-143">Select a user from the list.</span></span>
4. <span data-ttu-id="59fbf-144">ผู้ใช้ที่เลือก ให้เลือก **ภาพรวม** จากนั้นในแถบสั่ง ให้เลือก **รีเซ็ต** รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="59fbf-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="59fbf-145">เลือก **ปุ่มรีเซ็ต** รหัสผ่าน และปฏิบัติตามคําแนะนําบนหน้าจอ</span><span class="sxs-lookup"><span data-stu-id="59fbf-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="59fbf-146">เฉพาะการรีเซ็ตที่ผ่านพอร์ทัล **Azure เท่านั้น** ที่สนับสนุนการเขียนรหัสผ่านกลับ</span><span class="sxs-lookup"><span data-stu-id="59fbf-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="59fbf-147">**ฉันตั้งค่ารหัสผ่านของผู้ใช้ภายในองค์กรใหม่จากพอร์ทัลผู้ดูแลระบบ Office 365 หรือแอปพลิเคชัน Office 365 บนอุปกรณ์เคลื่อนที่ แต่ผู้ใช้ยังคงไม่สามารถลงชื่อเข้าใช้ได้**</span><span class="sxs-lookup"><span data-stu-id="59fbf-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="59fbf-148">Writeback รหัสผ่านไม่ได้รับการสนับสนุนในพอร์ทัลนี้</span><span class="sxs-lookup"><span data-stu-id="59fbf-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="59fbf-149">รีเซ็ตรหัสผ่านของผู้ใช้อีกครั้งในพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="59fbf-149">Reset the user's password again in the Azure portal.</span></span>
