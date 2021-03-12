---
title: มอบหมายบทบาทบันทึกการตรวจสอบในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายของ Office 365 &
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749525"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="3ad81-102">มอบหมายบทบาทบันทึกการตรวจสอบในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายของ Office 365 &</span><span class="sxs-lookup"><span data-stu-id="3ad81-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="3ad81-103">เมื่อต้องการค้นหาบันทึกการตรวจสอบ Office 365 ผู้ดูแลระบบต้องได้รับการ **มอบหมายบทบาทบันทึก** การตรวจสอบดูเท่านั้นหรือ **บทบาทบันทึก** การตรวจสอบใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="3ad81-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="3ad81-104">บทบาทเหล่านี้จะถูกมอบหมายให้กับกลุ่มบทบาทการจัดการการปฏิบัติตามกฎระเบียบและการจัดการองค์กรตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="3ad81-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="3ad81-105">ผู้ดูแลระบบส่วนกลางใน Office 365 และ Microsoft 365 จะถูกเพิ่มเป็นสมาชิกของกลุ่มบทบาทการจัดการองค์กรโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="3ad81-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="3ad81-106">เมื่อต้องการให้ผู้ใช้ค้นหาที่มีสิทธิ์ระดับต่สุด ให้สร้างกลุ่มบทบาทแบบมอบหมายเองใน Exchange Online เพิ่มบทบาทดูเท่านั้นบันทึกการตรวจสอบหรือบทบาทบันทึกการตรวจสอบ แล้วเพิ่มผู้ใช้เป็นสมาชิกของกลุ่มบทบาทใหม่</span><span class="sxs-lookup"><span data-stu-id="3ad81-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="3ad81-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and Search the audit log in the Security & Compliance [Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="3ad81-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>