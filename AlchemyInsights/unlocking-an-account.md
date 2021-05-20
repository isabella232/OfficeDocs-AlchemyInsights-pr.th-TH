---
title: การปลดล็อกบัญชี
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002449"
- "4748"
ms.openlocfilehash: cf2431cb49902b3f7625ab96bc6d4e2121e51fdd
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544163"
---
# <a name="unlocking-an-account"></a><span data-ttu-id="b4406-102">การปลดล็อกบัญชี</span><span class="sxs-lookup"><span data-stu-id="b4406-102">Unlocking an account</span></span>

<span data-ttu-id="b4406-103">ผู้ใช้อาจล็อกไม่เข้าMicrosoft 365เนื่องจากพยายามใส่รหัสผ่านไม่ดีหรือถูกโจมตีอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="b4406-103">It's possible users are locked out of Microsoft 365 due to bad password attempts or other compromises.</span></span> <span data-ttu-id="b4406-104">เมื่อต้องการช่วยให้ผู้ใช้ลงชื่อเข้าใช้Microsoft 365 **คุณสามารถลองขั้นตอนต่อไปนี้ก่อนที่จะเปิด การร้องขอ** การสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="b4406-104">To help users sign back in to Microsoft 365, **you can attempt the following steps before opening a Support Request**.</span></span> 

<span data-ttu-id="b4406-105">**อีเมลที่ถูกห้าม**</span><span class="sxs-lookup"><span data-stu-id="b4406-105">**Email Restricted**</span></span>

<span data-ttu-id="b4406-106">ในฐานะผู้ดูแลระบบ ถ้าผู้ใช้รายใดรายหนึ่งของคุณถูกห้ามการส่งอีเมล คุณสามารถ [ยกเลิกการบล็อกบัญชีได้](/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="b4406-106">As an admin, if one of your users is restricted from sending email, you can [unblock the account yourself](/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam).</span></span> <span data-ttu-id="b4406-107">ผู้ใช้จะสามารถส่งอีเมลภายในหนึ่งชั่วโมงหลังจากเอาข้อจํากัดออก</span><span class="sxs-lookup"><span data-stu-id="b4406-107">The user will be able to send email within an hour after removing the restriction.</span></span>

<span data-ttu-id="b4406-108">**ตั้งค่ารหัสผ่านผู้ใช้ใหม่**</span><span class="sxs-lookup"><span data-stu-id="b4406-108">**Reset the User Password**</span></span>

1. <span data-ttu-id="b4406-109">ในศูนย์การจัดการ ให้ไปที่ **ผู้ใช้ > [ผู้ใช้](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)** ที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="b4406-109">In the admin center, go to **Users > [Active Users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span></span>

2. <span data-ttu-id="b4406-110">เลือกผู้ใช้ แล้วคลิก **รีเซ็ต** รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="b4406-110">Select the user and click **Reset Password**.</span></span>

<span data-ttu-id="b4406-111">**ตรวจสอบให้แน่ใจว่าผู้ใช้สามารถลงชื่อเข้าใช้ได้**</span><span class="sxs-lookup"><span data-stu-id="b4406-111">**Make sure the user is allowed to sign in**</span></span>

1. <span data-ttu-id="b4406-112">ในศูนย์การจัดการ ให้ไปที่ **ผู้ใช้ > [ผู้ใช้](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)** ที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="b4406-112">In the admin center, go to **Users > [Active Users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span></span>

2. <span data-ttu-id="b4406-113">เลือกผู้ใช้ แล้วคลิกจุดสามจุด (การแอคชันเพิ่มเติม) แล้วคลิก **แก้ไขสถานะการเข้าสู่ระบบ**</span><span class="sxs-lookup"><span data-stu-id="b4406-113">Select the user and click the three dots (more actions), then click **Edit sign-in status**.</span></span>

<span data-ttu-id="b4406-114">For more password reset scenarios, including Self-Service Password Reset, [see Reset Microsoft 365 for multiple-attempts-to-charge-online-payment-instrumentsbusiness passwords](/microsoft-365/admin/add-users/reset-passwords).</span><span class="sxs-lookup"><span data-stu-id="b4406-114">For more password reset scenarios, including Self-Service Password Reset, see [Reset Microsoft 365 for multiple-attempts-to-charge-online-payment-instrumentsbusiness passwords](/microsoft-365/admin/add-users/reset-passwords).</span></span>

<span data-ttu-id="b4406-115">บริการนี้จะป้องกันไม่ให้ผู้ใช้ส่งอีเมลหลังจากตรวจพบหลักฐานของบัญชีที่ถูกละเมิด และ/หรือสแปมขาออก</span><span class="sxs-lookup"><span data-stu-id="b4406-115">The service prevents a user from sending email after detecting evidence of a compromised account and/or outbound spam.</span></span> <span data-ttu-id="b4406-116">เพื่อความปลอดภัย ให้ปฏิบัติตามขั้นตอนใน[การตอบกลับบัญชีผู้ใช้อีเมลที่ถูก](/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)ละเมิด Microsoft 365บัญชีผู้ใช้นั้น</span><span class="sxs-lookup"><span data-stu-id="b4406-116">As a precaution, follow the steps in [Responding to a Compromised Email Account in Microsoft 365](/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) for the user.</span></span>
