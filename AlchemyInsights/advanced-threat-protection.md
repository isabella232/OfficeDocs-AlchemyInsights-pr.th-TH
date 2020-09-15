---
title: การป้องกันการคุกคามขั้นสูงของ Office ๓๖๕
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1036
ms.assetid: ''
ms.openlocfilehash: c6b552a11b2eee647e2e5dc7b93523b03c0e7ea3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696640"
---
# <a name="office-365-advanced-threat-protection"></a><span data-ttu-id="1e3b2-102">การป้องกันการคุกคามขั้นสูงของ Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="1e3b2-102">Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="1e3b2-103">สิ่งที่แนบมาที่ปลอดภัยลิงก์ที่ปลอดภัยและการป้องกันฟิชชิ่งเป็นส่วนหนึ่งของ Office ๓๖๕การป้องกันภัยคุกคามขั้นสูง (ATP)</span><span class="sxs-lookup"><span data-stu-id="1e3b2-103">Safe Attachments, Safe Links, and anti-phishing are part of Office 365 Advanced Threat Protection (ATP).</span></span> <span data-ttu-id="1e3b2-104">Enterprise E5, การศึกษา A5 และ Microsoft ๓๖๕ Business Premium รวมเอทีพี</span><span class="sxs-lookup"><span data-stu-id="1e3b2-104">Enterprise E5, Education A5, and Microsoft 365 Business Premium include ATP.</span></span> <span data-ttu-id="1e3b2-105">แผนอื่นๆทั้งหมดจำเป็นต้องใช้การสมัครใช้งาน add-on ของ ATP</span><span class="sxs-lookup"><span data-stu-id="1e3b2-105">All other plans require an add-on ATP subscription.</span></span>

- <span data-ttu-id="1e3b2-106">คุณจำเป็นต้องกำหนดสิทธิ์การใช้งานที่เหมาะสมเพื่อปกป้องผู้ใช้ของคุณโดย Office ๓๖๕ ATP</span><span class="sxs-lookup"><span data-stu-id="1e3b2-106">You need to assign the appropriate licenses to protect your users by Office 365 ATP.</span></span> <span data-ttu-id="1e3b2-107">ให้ดู [หัวข้อนี้](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) สำหรับคำแนะนำเกี่ยวกับวิธีการนำสิทธิ์การใช้งานจำนวนมากไปใช้กับผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="1e3b2-107">See [this topic](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) for instructions on how to bulk apply licenses to your users.</span></span>

- <span data-ttu-id="1e3b2-108">ผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบความปลอดภัยสามารถเข้าถึงฟีเจอร์ของ Office ๓๖๕ ATP ในศูนย์**Threat Managmeent**การปฏิบัติตามนโยบาย & ด้านความปลอดภัยที่ \> **นโยบาย**Managmeent ของภัยคุกคาม</span><span class="sxs-lookup"><span data-stu-id="1e3b2-108">Global administrators or security administrators can access Office 365 ATP features in the Security & Compliance Center at **Threat Managmeent** \> **Policy**.</span></span>

- <span data-ttu-id="1e3b2-109">สิ่งที่แนบมาที่ปลอดภัยและนโยบายการเชื่อมโยงที่ปลอดภัยสามารถลักษณะคุณทั้งองค์กรโดเมนที่เฉพาะเจาะจงหรือกลุ่มผู้ใช้ที่มีขนาดเล็กลง</span><span class="sxs-lookup"><span data-stu-id="1e3b2-109">Safe Attachments and Safe Link policies can be scoped you your entire organization, specific domains, or smaller groups of users.</span></span>

- <span data-ttu-id="1e3b2-110">ไม่มีนโยบายสิ่งที่แนบมา ATP Safe ที่เป็นค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="1e3b2-110">There is no default ATP Safe Attachment policy.</span></span> <span data-ttu-id="1e3b2-111">คุณจำเป็นต้อง [สร้างนโยบาย](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-atp-safe-attachments-policies) และนำไปใช้กับผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="1e3b2-111">You need to [create a policy](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-atp-safe-attachments-policies) and apply it to your users.</span></span>

- <span data-ttu-id="1e3b2-112">นโยบายการเชื่อมโยงที่มีความปลอดภัย ATP เริ่มต้นที่นำไปใช้กับทุกคนในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="1e3b2-112">There is a default ATP Safe Links policy that applies to everyone in your organization.</span></span> <span data-ttu-id="1e3b2-113">เมื่อต้องการแก้ไขนโยบายนี้หรือเมื่อต้องการสร้างนโยบายแบบกำหนดเองให้ดู[หัวข้อนี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-atp-safe-links-policies)</span><span class="sxs-lookup"><span data-stu-id="1e3b2-113">To edit this policy or to create custom policies, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-atp-safe-links-policies).</span></span>
