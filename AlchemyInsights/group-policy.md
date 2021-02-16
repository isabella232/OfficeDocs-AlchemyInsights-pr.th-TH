---
title: นโยบายกลุ่ม
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
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256908"
---
# <a name="group-policy"></a><span data-ttu-id="69b12-102">นโยบายกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="69b12-102">Group policy</span></span>

<span data-ttu-id="69b12-103">การตั้งค่าวัตถุผู้ใช้และคอมพิวเตอร์ใน Azure Active Directory Domain Services (Azure AD DS) มักจะได้รับการจัดการโดยใช้ Group Policy Objects (GPOs)</span><span class="sxs-lookup"><span data-stu-id="69b12-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="69b12-104">Azure AD DS ประกอบด้วย GPOs ในตัวของผู้ใช้ AADDC และคอนเทนเนอร์คอมพิวเตอร์ AADDC</span><span class="sxs-lookup"><span data-stu-id="69b12-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="69b12-105">คุณสามารถกําหนดค่า GPOs ที่มีอยู่แล้วภายในเหล่านี้เพื่อกําหนดค่านโยบายกลุ่มตามที่ต้องการในสภาพแวดล้อมของคุณ</span><span class="sxs-lookup"><span data-stu-id="69b12-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="69b12-106">สมาชิกของกลุ่มผู้ดูแลระบบ Azure AD DC มีสิทธิ์การดูแลนโยบายกลุ่มในโดเมน Azure AD DS และยังสามารถสร้างหน่วย GPOs และหน่วยองค์กรแบบปรับแต่งเอง (OUs)</span><span class="sxs-lookup"><span data-stu-id="69b12-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="69b12-107">ดูข้อมูลเพิ่มเติมเกี่ยวกับนโยบายกลุ่มและวิธีใช้งาน ดู [ภาพรวมของ](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))นโยบายกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="69b12-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="69b12-108">ในสภาพแวดล้อมแบบไฮบริด นโยบายกลุ่มที่กําหนดค่าในสภาพแวดล้อม AD DS ภายในองค์กรจะไม่ถูกซิงโครไนซ์กับ Azure AD DS</span><span class="sxs-lookup"><span data-stu-id="69b12-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="69b12-109">เมื่อต้องการกําหนดการตั้งค่าการกําหนดค่าให้กับผู้ใช้หรือคอมพิวเตอร์ใน Azure AD DS ให้แก้ไขหนึ่งใน GPOs เริ่มต้นหรือสร้าง GPO แบบกําหนดเอง</span><span class="sxs-lookup"><span data-stu-id="69b12-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="69b12-110">บทความนี้ [จัดการนโยบายกลุ่ม](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) แสดงวิธีการติดตั้งเครื่องมือการจัดการนโยบายกลุ่ม วิธีที่ ton แก้ไข GPOs ในตัว และวิธีการสร้าง GPOs แบบปรับแต่งเอง</span><span class="sxs-lookup"><span data-stu-id="69b12-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



