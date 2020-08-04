---
title: ปัญหาในการใช้คอนโซลผู้ดูแลระบบ Intun
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555880"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="53004-102">ปัญหาในการใช้คอนโซลผู้ดูแลระบบ Intun</span><span class="sxs-lookup"><span data-stu-id="53004-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="53004-103">**"การเข้าถึงถูกปฏิเสธ"**</span><span class="sxs-lookup"><span data-stu-id="53004-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="53004-104">หากคุณเป็นสมาชิกของบทบาทแบบกําหนดเองของ Intunem ให้ตรวจสอบว่ามีการกําหนดสิทธิ์การใช้งาน Intun หรือ Enterprise Mobility Suite (EMS) ให้กับบัญชีของคุณ</span><span class="sxs-lookup"><span data-stu-id="53004-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="53004-105">ถ้าคุณกําลังใช้ตัวจัดการการตั้งค่าคอนฟิกเพื่อจัดการอุปกรณ์ ตรวจสอบคุณไม่ได้เป็นส่วนหนึ่งของคอลเลกชันผู้ใช้ Intun</span><span class="sxs-lookup"><span data-stu-id="53004-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="53004-106">ตรวจสอบว่า คุณได้รับการกําหนดสิทธิ์การควบคุมดูแลตามบทบาทที่เหมาะสม (RBAC) ในใบบังคับบทบาท Intun</span><span class="sxs-lookup"><span data-stu-id="53004-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="53004-107">ตรวจสอบว่ากลุ่มที่ใช้ไม่ใช่รายชื่อการแจกจ่าย</span><span class="sxs-lookup"><span data-stu-id="53004-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="53004-108">Intuner inพอร์ทัล Azure สนับสนุนเฉพาะบัญชีผู้ใช้ที่อยู่ในกลุ่มความปลอดภัยของ Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="53004-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="53004-109">ตรวจทานกลุ่มของคุณในพอร์ทัล Azure >กลุ่ม**Intun หรือ**  >  **Groups**ในพอร์ทัล Azure >**ไดเรกทอรีที่ใช้งานอยู่ของ Azure**</span><span class="sxs-lookup"><span data-stu-id="53004-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="53004-110">**ผู้ใช้มีสิทธิ์มากเกินไปสําหรับบทบาท Intun**</span><span class="sxs-lookup"><span data-stu-id="53004-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="53004-111">แนะนําให้ผู้ใช้ไปที่บทบาท**Intune**  >  **Intuner Intun**  >  **My permissions**  >  **Export**</span><span class="sxs-lookup"><span data-stu-id="53004-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="53004-112">**ฉันได้เพิ่มกลุ่มขอบเขตลงในบทบาท แต่ผู้ใช้ในบทบาทนั้นยังคงเห็นผู้ใช้หรืออุปกรณ์อื่นๆ**</span><span class="sxs-lookup"><span data-stu-id="53004-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="53004-113">กลุ่มขอบเขตไม่กรองผู้ใช้หรืออุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="53004-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="53004-114">กลุ่มขอบเขต:</span><span class="sxs-lookup"><span data-stu-id="53004-114">Scope groups:</span></span>

- <span data-ttu-id="53004-115">จํากัดผู้ที่สามารถกําหนดนโยบายหรือแอปพลิเคชันได้</span><span class="sxs-lookup"><span data-stu-id="53004-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="53004-116">อนุญาตให้เฉพาะผู้ใช้เฉพาะรายเท่านั้นที่จะเรียกใช้งานระยะไกลบนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="53004-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="53004-117">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับกลุ่มขอบเขต ให้ดูที่[การควบคุมการเข้าถึงตามบทบาท (RBAC) ด้วย Microsoft Intun](https://docs.microsoft.com/intune/role-based-access-control)</span><span class="sxs-lookup"><span data-stu-id="53004-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="53004-118">**ฉันเพิ่มผู้ใช้ในบทบาท Intun**</span><span class="sxs-lookup"><span data-stu-id="53004-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="53004-119">นําทางไปยัง Intun>**ผู้ใช้**ในพอร์ทัล Azure และตรวจสอบว่า ผู้ใช้ไม่ได้กําหนดให้กับบทบาทต่อไปนี้ในพอร์ทัล Azure:</span><span class="sxs-lookup"><span data-stu-id="53004-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="53004-120">ผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="53004-120">Global administrator</span></span>
- <span data-ttu-id="53004-121">ผู้ดูแลบริการ Intun</span><span class="sxs-lookup"><span data-stu-id="53004-121">Intune service administrator</span></span>
- <span data-ttu-id="53004-122">ผู้ดูแล SharePoint</span><span class="sxs-lookup"><span data-stu-id="53004-122">SharePoint administrator</span></span>

<span data-ttu-id="53004-123">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การควบคุมการเข้าถึงตามบทบาท (RBAC) ด้วย Microsoft Intun](https://docs.microsoft.com/intune/role-based-access-control)</span><span class="sxs-lookup"><span data-stu-id="53004-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="53004-124">**ปัญหาการเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="53004-124">**Access Issues**</span></span>

<span data-ttu-id="53004-125">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[คุณไม่สามารถลงชื่อเข้าใช้ Office 365, Azure หรือ Intun](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)</span><span class="sxs-lookup"><span data-stu-id="53004-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>