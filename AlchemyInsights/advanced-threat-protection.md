---
title: การป้องกันภัยคุกคามขั้นสูงของ Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1036
ms.assetid: ''
ms.openlocfilehash: 5fc3f30e1f08764393dcced94be541b1c6bcc84d
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506613"
---
# <a name="office-365-advanced-threat-protection"></a><span data-ttu-id="e6d51-102">การป้องกันภัยคุกคามขั้นสูงของ Office 365</span><span class="sxs-lookup"><span data-stu-id="e6d51-102">Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="e6d51-103">สิ่งที่แนบมาที่ปลอดภัย, การเชื่อมโยงที่ปลอดภัย, และการป้องกันฟิชชิ่งเป็นส่วนหนึ่งของการป้องกันภัยคุกคามขั้นสูงของ Office 365 (ATP)</span><span class="sxs-lookup"><span data-stu-id="e6d51-103">Safe Attachments, Safe Links, and anti-phishing are part of Office 365 Advanced Threat Protection (ATP).</span></span> <span data-ttu-id="e6d51-104">องค์กร E5, การศึกษา A5 และ Microsoft 365 พรีเมี่ยมธุรกิจรวมถึง ATP</span><span class="sxs-lookup"><span data-stu-id="e6d51-104">Enterprise E5, Education A5, and Microsoft 365 Business Premium include ATP.</span></span> <span data-ttu-id="e6d51-105">แผนอื่นๆ ทั้งหมดจําเป็นต้องมีการสมัครใช้บริการ ATP แบบแอดออน</span><span class="sxs-lookup"><span data-stu-id="e6d51-105">All other plans require an add-on ATP subscription.</span></span>

- <span data-ttu-id="e6d51-106">คุณต้องมอบหมายสิทธิ์การใช้งานที่เหมาะสมเพื่อปกป้องผู้ใช้ของคุณโดย Atp ของ Office 365</span><span class="sxs-lookup"><span data-stu-id="e6d51-106">You need to assign the appropriate licenses to protect your users by Office 365 ATP.</span></span> <span data-ttu-id="e6d51-107">ดู[หัวข้อนี้](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)สําหรับคําแนะนําเกี่ยวกับวิธีการใช้สิทธิ์การใช้งานจํานวนมากกับผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="e6d51-107">See [this topic](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) for instructions on how to bulk apply licenses to your users.</span></span>

- <span data-ttu-id="e6d51-108">ผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบความปลอดภัยสามารถเข้าถึงคุณลักษณะของ Office 365 ATP ในศูนย์การปฏิบัติตามกฎระเบียบ&ความปลอดภัยที่นโยบาย**การจัดการภัยคุกคาม** \> **Policy**</span><span class="sxs-lookup"><span data-stu-id="e6d51-108">Global administrators or security administrators can access Office 365 ATP features in the Security & Compliance Center at **Threat Managmeent** \> **Policy**.</span></span>

- <span data-ttu-id="e6d51-109">นโยบายของสิ่งที่แนบมาที่ปลอดภัยและนโยบายการเชื่อมโยงที่ปลอดภัยสามารถกําหนดขอบเขตองค์กรของคุณทั้งองค์กร</span><span class="sxs-lookup"><span data-stu-id="e6d51-109">Safe Attachments and Safe Link policies can be scoped you your entire organization, specific domains, or smaller groups of users.</span></span>

- <span data-ttu-id="e6d51-110">ไม่มีนโยบายความปลอดภัย ATP เริ่มต้นสิ่งที่แนบมา</span><span class="sxs-lookup"><span data-stu-id="e6d51-110">There is no default ATP Safe Attachment policy.</span></span> <span data-ttu-id="e6d51-111">คุณต้อง[สร้างนโยบาย](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-atp-safe-attachments-policies)และนําไปใช้กับผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="e6d51-111">You need to [create a policy](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-atp-safe-attachments-policies) and apply it to your users.</span></span>

- <span data-ttu-id="e6d51-112">มีนโยบาย ATP Safe Links เริ่มต้นที่ใช้กับทุกคนในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="e6d51-112">There is a default ATP Safe Links policy that applies to everyone in your organization.</span></span> <span data-ttu-id="e6d51-113">เมื่อต้องการแก้ไขนโยบายนี้ หรือสร้างนโยบายแบบกําหนดเอง ให้ดูที่[หัวข้อนี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-atp-safe-links-policies)</span><span class="sxs-lookup"><span data-stu-id="e6d51-113">To edit this policy or to create custom policies, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-atp-safe-links-policies).</span></span>
