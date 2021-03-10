---
title: ปัญหาในการรีเซ็ตรหัสผ่าน
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696280"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="f2831-102">ปัญหาในการรีเซ็ตรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="f2831-102">Problems resetting password</span></span>

<span data-ttu-id="f2831-103">ต่อไปนี้คือบางปัญหาที่คุณอาจพบเมื่อรีเซ็ตรหัสผ่านและวิธีแก้ไขปัญหาที่เป็นไปได้:</span><span class="sxs-lookup"><span data-stu-id="f2831-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="f2831-104">**ฉันมีปัญหากับการรีเซ็ตรหัสผ่านไม่ครอบคลุมอยู่ในประเภทอื่นๆ**</span><span class="sxs-lookup"><span data-stu-id="f2831-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="f2831-105">ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้รีเซ็ตรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="f2831-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="f2831-106">เฉพาะผู้ดูแลระบบส่วนกลาง รหัสผ่าน และผู้ดูแลระบบของผู้ใช้เท่านั้นที่สามารถตั้งค่ารหัสผ่านผู้ใช้ใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="f2831-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="f2831-107">ผู้ดูแลระบบส่วนกลางยังสามารถตั้งค่ารหัสผ่านของผู้ดูแลระบบที่มีสิทธิ์ใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="f2831-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="f2831-108">โปรดแน่ใจว่าคุณเข้าใจความต้องการด้านสิทธิ์การใช้งาน:</span><span class="sxs-lookup"><span data-stu-id="f2831-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="f2831-109">คุณต้องมีอย่างน้อยหนึ่งสิทธิ์การใช้งานที่มอบหมายในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="f2831-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="f2831-110">ระบบคลาวด์เฉพาะผู้ใช้ - Office 365 (O365) ชําระเงิน SKU หรือ Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="f2831-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="f2831-111">ผู้ใช้ระบบคลาวด์และ/หรือผู้ใช้ในองค์กร - Azure AD Premium P1 หรือ P2, Enterprise Mobility + Security (EMS) หรือ Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="f2831-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="f2831-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f2831-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f2831-113">**ฉันพบปัญหาในการทดสอบนโยบายการตั้งค่ารหัสผ่านใหม่ที่ฉันตั้งค่าไว้**</span><span class="sxs-lookup"><span data-stu-id="f2831-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="f2831-114">นโยบายที่ปรับใช้ล่าสุดอาจใช้เวลาหลายนาทีเพื่อคัดลอกข้อมูลทั้งหมดและจุดสิ้นสุด</span><span class="sxs-lookup"><span data-stu-id="f2831-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="f2831-115">ระยะทางจริงจากศูนย์ข้อมูลจะส่งผลต่อวิธีการปรับใช้การเปลี่ยนแปลงอย่างรวดเร็วด้วย</span><span class="sxs-lookup"><span data-stu-id="f2831-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="f2831-116">ทดสอบกับผู้ใช้ไม่ใช่ผู้ดูแลระบบ และทดสอบกับผู้ใช้กลุ่มเล็กๆ</span><span class="sxs-lookup"><span data-stu-id="f2831-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="f2831-117">นโยบายที่กําหนดค่าในพอร์ทัล Azure จะใช้กับผู้ใช้เท่านั้น ไม่ใช่ผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="f2831-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="f2831-118">Microsoft บังคับใช้นโยบายรีเซ็ตรหัสผ่านสองทางเริ่มต้นอย่างรัดกุมให้กับบทบาทผู้ดูแลระบบ Azure (ตัวอย่าง: ผู้ดูแลระบบส่วนกลาง ผู้ดูแลระบบฝ่ายสนับสนุน ผู้ดูแลระบบรหัสผ่าน เป็นต้น)</span><span class="sxs-lookup"><span data-stu-id="f2831-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="f2831-119">เรียนรู้เพ [ิ่มเติมเกี่ยวกับนโยบายของ](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)ผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="f2831-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="f2831-120">**ฉันต้องการปรับใช้การรีเซ็ตรหัสผ่าน แต่ฉันไม่ต้องการให้ผู้ใช้ของฉันลงทะเบียนข้อมูลความปลอดภัยเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="f2831-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="f2831-121">ใส่ข้อมูลล่วงหน้าให้กับผู้ใช้ของคุณ เพื่อให้พวกเขาไม่ต้องใส่ข้อมูลเหล่านั้น!</span><span class="sxs-lookup"><span data-stu-id="f2831-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="f2831-122">- ในฐานะผู้ดูแลระบบ คุณสามารถตั้งค่าคุณสมบัติโทรศัพท์และอีเมลให้กับผู้ใช้ของคุณก่อนที่จะเริ่มใช้การตั้งค่ารหัสผ่านใหม่ให้กับองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="f2831-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="f2831-123">คุณสามารถลองใช้ API, PowerShell หรือ Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="f2831-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="f2831-124">ข้อมูลเพิ่มเติมที่นี่:</span><span class="sxs-lookup"><span data-stu-id="f2831-124">More information here:</span></span>
- [<span data-ttu-id="f2831-125">การปรับใช้การรีเซ็ตรหัสผ่านโดยไม่ให้ผู้ใช้ลงทะเบียน</span><span class="sxs-lookup"><span data-stu-id="f2831-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="f2831-126">การรีเซ็ตรหัสผ่านจะใช้ข้อมูลใด</span><span class="sxs-lookup"><span data-stu-id="f2831-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="f2831-127">**ปุ่มรีเซ็ตรหัสผ่านเป็นสีเทา**</span><span class="sxs-lookup"><span data-stu-id="f2831-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="f2831-128">คุณไม่ได้รับอนุญาตให้รีเซ็ตรหัสผ่านของผู้ใช้นี้</span><span class="sxs-lookup"><span data-stu-id="f2831-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="f2831-129">เฉพาะผู้ดูแลระบบส่วนกลาง รหัสผ่าน และผู้ดูแลระบบของผู้ใช้เท่านั้นที่สามารถตั้งค่ารหัสผ่านผู้ใช้ใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="f2831-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="f2831-130">ผู้ดูแลระบบส่วนกลางยังสามารถตั้งค่ารหัสผ่านของผู้ดูแลระบบที่มีสิทธิ์ใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="f2831-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="f2831-131">**ฉันไม่เห็นใบรีเซ็ตรหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="f2831-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="f2831-132">คุณไม่ได้รับอนุญาตให้ตั้งค่ารหัสผ่านใหม่</span><span class="sxs-lookup"><span data-stu-id="f2831-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="f2831-133">เฉพาะผู้ดูแลระบบส่วนกลาง รหัสผ่าน และผู้ดูแลระบบของผู้ใช้เท่านั้นที่สามารถตั้งค่ารหัสผ่านผู้ใช้ใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="f2831-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="f2831-134">ผู้ดูแลระบบส่วนกลางยังสามารถตั้งค่ารหัสผ่านของผู้ดูแลระบบที่มีสิทธิ์ใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="f2831-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="f2831-135">**ฉันไม่เห็นใบผสานภายในองค์กรในการรีเซ็ตรหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="f2831-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="f2831-136">ใบผสานภายในองค์กรจะปรากฏเฉพาะในสภาพแวดล้อมแบบไฮบริดเท่านั้น หมายความว่าคุณใช้ Writeback ของรหัสผ่านเพื่อจัดการรหัสผ่านของผู้ใช้ภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="f2831-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="f2831-137">คุณไม่เห็นใบนี้หาก:</span><span class="sxs-lookup"><span data-stu-id="f2831-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="f2831-138">คุณไม่ได้ใช้ Writeback รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="f2831-138">You are not using password writeback</span></span>
    - <span data-ttu-id="f2831-139">มีปัญหากับการติดตั้ง/การเชื่อมต่อของ Writeback รหัสผ่านของคุณ</span><span class="sxs-lookup"><span data-stu-id="f2831-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="f2831-140">มีปัญหากับการติดตั้ง/การเชื่อมต่อ Azure AD Connect ของคุณ</span><span class="sxs-lookup"><span data-stu-id="f2831-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="f2831-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="f2831-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="f2831-142">**ฉันไม่รู้วิธีรีเซ็ตรหัสผ่านของผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="f2831-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="f2831-143">ลงชื่อเข้าใช้พอร์ทัล Azure ในฐานะผู้ดูแลระบบที่เหมาะสม</span><span class="sxs-lookup"><span data-stu-id="f2831-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="f2831-144">ไปที่ Blade ผู้ใช้และกลุ่ม **เลือก ผู้ใช้** ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="f2831-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="f2831-145">เลือกผู้ใช้จากรายการ</span><span class="sxs-lookup"><span data-stu-id="f2831-145">Select a user from the list.</span></span>
1. <span data-ttu-id="f2831-146">ผู้ใช้ที่เลือก ให้เลือก **ภาพรวม** จากนั้นในแถบสั่ง ให้คลิก **รีเซ็ต** รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="f2831-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="f2831-147">ปฏิบัติตามคําแนะนําบนหน้าจอ</span><span class="sxs-lookup"><span data-stu-id="f2831-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="f2831-148">เฉพาะการรีเซ็ตที่ผ่านพอร์ทัล Azure เท่านั้นที่สนับสนุนการเขียนรหัสผ่านกลับ</span><span class="sxs-lookup"><span data-stu-id="f2831-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="f2831-149">**ฉันตั้งค่ารหัสผ่านของผู้ใช้ภายในองค์กรใหม่จากพอร์ทัลผู้ดูแลระบบ Office 365 หรือแอปพลิเคชัน Office 365 บนอุปกรณ์เคลื่อนที่ แต่ผู้ใช้ยังคงไม่สามารถลงชื่อเข้าใช้ได้**</span><span class="sxs-lookup"><span data-stu-id="f2831-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="f2831-150">Writeback รหัสผ่านไม่ได้รับการสนับสนุนในพอร์ทัลนี้</span><span class="sxs-lookup"><span data-stu-id="f2831-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="f2831-151">รีเซ็ตรหัสผ่านของผู้ใช้อีกครั้งในพอร์ทัล Azure - portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="f2831-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

