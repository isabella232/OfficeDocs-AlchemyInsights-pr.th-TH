---
title: เปิดใช้งานการรับรองความถูกต้องและการแก้ไขปัญหา SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077670"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="66a65-102">เปิดใช้งานการรับรองความถูกต้องและการแก้ไขปัญหา SMTP</span><span class="sxs-lookup"><span data-stu-id="66a65-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="66a65-103">ถ้าคุณต้องการเปิดใช้งานการรับรองความถูกต้อง SMTP ให้กับกล่องจดหมาย หรือคุณได้รับข้อผิดพลาด "ไคลเอ็นต์ไม่ได้รับการรับรองความถูกต้อง", "การรับรองความถูกต้องไม่ส", หรือ "SmtpClientAuthentication" ที่มีรหัส 5.7.57 หรือ 5.7.3 หรือ 5.7.139 เมื่อคุณพยายามรีเลย์อีเมลโดยการรับรองความถูกต้องอุปกรณ์หรือแอปพลิเคชันด้วย Microsoft 365 ให้ปฏิบัติสามอย่างเหล่านี้เพื่อแก้ไขปัญหา:</span><span class="sxs-lookup"><span data-stu-id="66a65-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="66a65-104">ปิดใช้งาน [ค่าเริ่มต้นความปลอดภัยของ Azure](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)โดยการสลับ **เปิดใช้งานค่าเริ่มต้นด้านความปลอดภัย\*\*\*\*เป็น** ไม่</span><span class="sxs-lookup"><span data-stu-id="66a65-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="66a65-105">a.</span><span class="sxs-lookup"><span data-stu-id="66a65-105">a.</span></span> <span data-ttu-id="66a65-106">ลงชื่อเข้าใช้พอร์ทัล Azure ในฐานะผู้ดูแลระบบความปลอดภัย ผู้ดูแลการเข้าถึงตามเงื่อนไข หรือผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="66a65-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="66a65-107">b.</span><span class="sxs-lookup"><span data-stu-id="66a65-107">b.</span></span> <span data-ttu-id="66a65-108">เรียกดูAzure Active Directory > **คุณสมบัติ**</span><span class="sxs-lookup"><span data-stu-id="66a65-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="66a65-109">c.</span><span class="sxs-lookup"><span data-stu-id="66a65-109">c.</span></span> <span data-ttu-id="66a65-110">เลือก **จัดการค่าเริ่มต้น** ความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="66a65-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="66a65-111">d.</span><span class="sxs-lookup"><span data-stu-id="66a65-111">d.</span></span> <span data-ttu-id="66a65-112">ตั้งค่า **เปิดใช้งานค่าเริ่มต้นความปลอดภัย\*\*\*\*เป็น** ไม่</span><span class="sxs-lookup"><span data-stu-id="66a65-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="66a65-113">e.</span><span class="sxs-lookup"><span data-stu-id="66a65-113">e.</span></span> <span data-ttu-id="66a65-114">เลือกบันทึก</span><span class="sxs-lookup"><span data-stu-id="66a65-114">Select **Save**.</span></span>

2. <span data-ttu-id="66a65-115">[เปิดใช้งานการส่ง SMTP](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) ไคลเอ็นต์บนกล่องจดหมายที่มีสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="66a65-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="66a65-116">a.</span><span class="sxs-lookup"><span data-stu-id="66a65-116">a.</span></span> <span data-ttu-id="66a65-117">จากรายการศูนย์การจัดการ Microsoft 365 ให้ไปที่ **ผู้ใช้** ที่ใช้งานอยู่ แล้วเลือกผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="66a65-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="66a65-118">b.</span><span class="sxs-lookup"><span data-stu-id="66a65-118">b.</span></span> <span data-ttu-id="66a65-119">ไปที่แท็บ จดหมาย และ **ภายใต้ แอปอีเมล** ให้เลือก **จัดการแอป** อีเมล</span><span class="sxs-lookup"><span data-stu-id="66a65-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="66a65-120">d.</span><span class="sxs-lookup"><span data-stu-id="66a65-120">d.</span></span> <span data-ttu-id="66a65-121">ตรวจสอบให้แน่ใจว่า **มีการตรวจสอบ SMTP** ที่ได้รับการรับรองความถูกต้อง (เปิดใช้งาน)</span><span class="sxs-lookup"><span data-stu-id="66a65-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="66a65-122">e.</span><span class="sxs-lookup"><span data-stu-id="66a65-122">e.</span></span> <span data-ttu-id="66a65-123">เลือก **บันทึก** การเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="66a65-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="66a65-124">[ปิดใช้งานการรับรองความถูกต้องโดยใช้หลายปัจจัย (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) บนกล่องจดหมายที่มีสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="66a65-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="66a65-125">a.</span><span class="sxs-lookup"><span data-stu-id="66a65-125">a.</span></span> <span data-ttu-id="66a65-126">ไปที่ตัวเลือก ศูนย์การจัดการ Microsoft 365 และในเมนูการนําทางด้านซ้าย ให้เลือก **ผู้ใช้**  >  **ที่ใช้งานอยู่**</span><span class="sxs-lookup"><span data-stu-id="66a65-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="66a65-127">b.</span><span class="sxs-lookup"><span data-stu-id="66a65-127">b.</span></span> <span data-ttu-id="66a65-128">เลือก **การรับรองความถูกต้องโดยใช้หลาย** ปัจจัย</span><span class="sxs-lookup"><span data-stu-id="66a65-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="66a65-129">c.</span><span class="sxs-lookup"><span data-stu-id="66a65-129">c.</span></span> <span data-ttu-id="66a65-130">เลือกผู้ใช้และ **ปิดใช้งานการรับรองความถูกต้องโดยใช้หลาย** ปัจจัย</span><span class="sxs-lookup"><span data-stu-id="66a65-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
