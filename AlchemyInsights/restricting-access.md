---
title: การจำกัดการเข้าถึง
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7769"
ms.openlocfilehash: 8af9546f219474e2382cd2436470385bf3ad31e8
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015011"
---
# <a name="restricting-access"></a><span data-ttu-id="79ec3-102">การจำกัดการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="79ec3-102">Restricting access</span></span>

1. <span data-ttu-id="79ec3-103">สำหรับข้อมูลเกี่ยวกับวิธีการจำกัดการเข้าถึงแอปพลิเคชันให้ดู[ที่วิธีการ: จำกัดแอป AZURE ad ของคุณให้เป็นชุดของผู้ใช้ในผู้เช่า AZURE AD](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users)</span><span class="sxs-lookup"><span data-stu-id="79ec3-103">For information on how to restrict access to an application, see [How to: Restrict your Azure AD app to a set of users in an Azure AD tenant](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users).</span></span>
1. <span data-ttu-id="79ec3-104">เรียนรู้วิธีการตรวจสอบและจัดการสิทธิ์ของแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="79ec3-104">Learn how to review and manage application permissions.</span></span> <span data-ttu-id="79ec3-105">[ดำเนินการกับแอปพลิเคชัน overprivileged หรือแอปพลิเคชันที่น่าสงสัยใน Azure Active directory](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-application-permissions#control-access-to-an-application) มีการดำเนินการที่แตกต่างกันที่คุณสามารถดำเนินการเพื่อรักษาความปลอดภัยแอปพลิเคชันของคุณตามสถานการณ์สมมติ</span><span class="sxs-lookup"><span data-stu-id="79ec3-105">[Take action on overprivileged or suspicious applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-application-permissions#control-access-to-an-application) provides different actions you can take to secure your application according to the scenario.</span></span> <span data-ttu-id="79ec3-106">การดำเนินการเหล่านี้จะนำไปใช้กับแอปพลิเคชันทั้งหมดที่ถูกเพิ่มลงในผู้เช่า Azure Active directory (Azure AD) ของคุณผ่านทางผู้ใช้หรือความยินยอมของผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="79ec3-106">These actions apply to all applications that were added to your Azure Active Directory (Azure AD) tenant via user or admin consent.</span></span>
1. <span data-ttu-id="79ec3-107">[จัดการงานที่มอบหมายของผู้ใช้สำหรับแอปใน Azure Active directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal#configure-an-application-to-require-user-assignment) แสดงวิธีการกำหนดผู้ใช้และกลุ่มให้กับแอปพลิเคชันสำหรับองค์กรใน Azure active Directory (azure AD) จากภายในพอร์ทัล azure หรือโดยใช้ PowerShell</span><span class="sxs-lookup"><span data-stu-id="79ec3-107">[Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal#configure-an-application-to-require-user-assignment) shows you how to assign users, and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell.</span></span> <span data-ttu-id="79ec3-108">เมื่อคุณกำหนดผู้ใช้ให้กับแอปพลิเคชันแอปพลิเคชันจะปรากฏในแอปของผู้ใช้ของฉันเพื่อให้เข้าถึงได้ง่าย</span><span class="sxs-lookup"><span data-stu-id="79ec3-108">When you assign a user to an application, the application appears in the user's My Apps for easy access.</span></span> <span data-ttu-id="79ec3-109">ถ้าแอปพลิเคชัน exposes บทบาทคุณยังสามารถกำหนดบทบาทที่เฉพาะเจาะจงให้กับผู้ใช้ได้ด้วย</span><span class="sxs-lookup"><span data-stu-id="79ec3-109">If the application exposes roles, you can also assign a specific role to the user.</span></span>
    - <span data-ttu-id="79ec3-110">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการกำหนดผู้ใช้และกลุ่มให้ดูที่การ[เข้าถึงแบบมีเงื่อนไข: ผู้ใช้และกลุ่ม](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-users-groups)</span><span class="sxs-lookup"><span data-stu-id="79ec3-110">For more information on User and Group assignment see [Conditional Access: Users and groups](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-users-groups).</span></span>
