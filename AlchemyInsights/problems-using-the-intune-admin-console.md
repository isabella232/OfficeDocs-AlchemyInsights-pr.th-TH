---
title: ปัญหาในการใช้คอนโซลผู้ดูแลระบบของ Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728306"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="6d2ff-102">ปัญหาในการใช้คอนโซลผู้ดูแลระบบของ Intune</span><span class="sxs-lookup"><span data-stu-id="6d2ff-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="6d2ff-103">**"การเข้าถึงถูกปฏิเสธ" เมื่อนำทางพอร์ทัลผู้ดูแลระบบของ Intune**</span><span class="sxs-lookup"><span data-stu-id="6d2ff-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="6d2ff-104">ถ้าคุณเป็นสมาชิกของบทบาทแบบกำหนดเองของ Intune ให้ตรวจสอบให้แน่ใจว่ามีการกำหนดสิทธิ์การใช้งาน Intune หรือองค์กรการเคลื่อนไหวของ Intune (EMS) ให้กับบัญชีผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="6d2ff-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="6d2ff-105">ถ้าคุณกำลังใช้ตัวจัดการการกำหนดค่าเพื่อจัดการอุปกรณ์ให้ตรวจสอบว่าคุณไม่ได้เป็นส่วนหนึ่งของคอลเลกชันของผู้ใช้ Intune สำหรับตัวจัดการการกำหนดค่า MDM</span><span class="sxs-lookup"><span data-stu-id="6d2ff-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="6d2ff-106">ตรวจสอบว่าคุณได้รับสิทธิ์ที่เหมาะสมตามบทบาทการจัดการการดูแลระบบ (RBAC) ในใบมีดบทบาท Intune</span><span class="sxs-lookup"><span data-stu-id="6d2ff-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="6d2ff-107">การตรวจสอบความถูกต้องของกลุ่มที่ใช้ไม่ใช่รายชื่อการแจกจ่าย</span><span class="sxs-lookup"><span data-stu-id="6d2ff-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="6d2ff-108">Intune ในพอร์ทัล Azure สนับสนุนเฉพาะบัญชีผู้ใช้ที่เป็นสมาชิกของกลุ่มความปลอดภัยของ Azure Active directory เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="6d2ff-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="6d2ff-109">ตรวจทานกลุ่มของคุณในกลุ่มของ azure portal > **Intune**  >  **Groups**หรือใน azure portal > **azure active directory**</span><span class="sxs-lookup"><span data-stu-id="6d2ff-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="6d2ff-110">**ผู้ใช้มีสิทธิ์มากเกินไปสำหรับบทบาท Intune ที่ได้รับมอบหมาย**</span><span class="sxs-lookup"><span data-stu-id="6d2ff-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="6d2ff-111">แนะนำให้ผู้ใช้ไปที่บทบาท**intune**intune  >  **Intune roles**  >  **ของฉัน**  >  การ**ส่งออก**สิทธิ์ของฉันเพื่อตรวจทานสิทธิ์ที่ได้รับอนุญาต</span><span class="sxs-lookup"><span data-stu-id="6d2ff-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="6d2ff-112">**ฉันเพิ่มกลุ่มขอบเขตให้กับบทบาทแต่ผู้ใช้ในบทบาทนั้นยังคงเห็นผู้ใช้หรืออุปกรณ์อื่นๆ**</span><span class="sxs-lookup"><span data-stu-id="6d2ff-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="6d2ff-113">กลุ่มขอบเขตไม่กรองผู้ใช้หรืออุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="6d2ff-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="6d2ff-114">กลุ่มขอบเขต:</span><span class="sxs-lookup"><span data-stu-id="6d2ff-114">Scope groups:</span></span>

- <span data-ttu-id="6d2ff-115">จำกัดผู้ใช้ที่สามารถกำหนดนโยบายหรือแอปพลิเคชันให้กับผู้ใช้ได้</span><span class="sxs-lookup"><span data-stu-id="6d2ff-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="6d2ff-116">อนุญาตเฉพาะผู้ใช้ที่เฉพาะเจาะจงในการเรียกใช้งานระยะไกลบนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="6d2ff-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="6d2ff-117">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับกลุ่มขอบเขตให้ดู[ที่การควบคุมการเข้าถึงตามบทบาท (RBAC) ด้วย Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control)</span><span class="sxs-lookup"><span data-stu-id="6d2ff-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="6d2ff-118">**ฉันเพิ่มผู้ใช้ลงในบทบาทของ Intune แต่พวกเขายังมีสิทธิ์การเข้าถึงคอนโซลผู้ดูแลระบบ Intune แบบเต็ม**</span><span class="sxs-lookup"><span data-stu-id="6d2ff-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="6d2ff-119">นำทางไปยัง Intune > **ผู้ใช้** ในพอร์ทัล azure และตรวจสอบว่าผู้ใช้ไม่ได้รับมอบหมายให้กับบทบาทใดๆต่อไปนี้ในพอร์ทัล azure:</span><span class="sxs-lookup"><span data-stu-id="6d2ff-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="6d2ff-120">ผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="6d2ff-120">Global administrator</span></span>
- <span data-ttu-id="6d2ff-121">ผู้ดูแลระบบบริการ Intune</span><span class="sxs-lookup"><span data-stu-id="6d2ff-121">Intune service administrator</span></span>
- <span data-ttu-id="6d2ff-122">ผู้ดูแลระบบ SharePoint</span><span class="sxs-lookup"><span data-stu-id="6d2ff-122">SharePoint administrator</span></span>

<span data-ttu-id="6d2ff-123">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การควบคุมการเข้าถึงตามบทบาท (RBAC) ด้วย Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control)</span><span class="sxs-lookup"><span data-stu-id="6d2ff-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="6d2ff-124">**ปัญหาในการเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="6d2ff-124">**Access Issues**</span></span>

<span data-ttu-id="6d2ff-125">สำหรับข้อมูลเพิ่มเติมให้ดู [ที่คุณไม่สามารถลงชื่อเข้าใช้ Office ๓๖๕, Azure หรือ Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)ได้</span><span class="sxs-lookup"><span data-stu-id="6d2ff-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>