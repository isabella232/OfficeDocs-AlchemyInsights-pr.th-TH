---
title: การป้องกันภัยคุกคามขั้นสูงของ Office ๓๖๕
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1036
ms.assetid: ''
ms.openlocfilehash: ec9e74a1c1054d45356b8347a87e36c592c47fbf
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36664519"
---
# <a name="office-365-advanced-threat-protection"></a><span data-ttu-id="cdf15-102">การป้องกันภัยคุกคามขั้นสูงของ Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="cdf15-102">Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="cdf15-103">สิ่งที่แนบมาอย่างปลอดภัย, การเชื่อมโยงที่ปลอดภัยและการป้องกันฟิชชิ่งเป็นส่วนหนึ่งของ Office ๓๖๕การป้องกันภัยคุกคามขั้นสูง (ATP)</span><span class="sxs-lookup"><span data-stu-id="cdf15-103">Safe Attachments, Safe Links, and anti-phishing are part of Office 365 Advanced Threat Protection (ATP).</span></span> <span data-ttu-id="cdf15-104">องค์กร E5, การศึกษา A5 และ Microsoft ๓๖๕ธุรกิจรวมถึง ATP</span><span class="sxs-lookup"><span data-stu-id="cdf15-104">Enterprise E5, Education A5, and Microsoft 365 Business include ATP.</span></span> <span data-ttu-id="cdf15-105">แผนอื่นๆทั้งหมดต้องใช้การสมัครใช้งาน ATP add-on</span><span class="sxs-lookup"><span data-stu-id="cdf15-105">All other plans require an add-on ATP subscription.</span></span>

- <span data-ttu-id="cdf15-106">คุณจำเป็นต้องกำหนดใบอนุญาตที่เหมาะสมเพื่อป้องกันผู้ใช้ของคุณโดย Office ๓๖๕ ATP</span><span class="sxs-lookup"><span data-stu-id="cdf15-106">You need to assign the appropriate licenses to protect your users by Office 365 ATP.</span></span> <span data-ttu-id="cdf15-107">ดู[หัวข้อนี้](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users)สำหรับคำแนะนำเกี่ยวกับวิธีการใช้ใบอนุญาตจำนวนมากกับผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="cdf15-107">See [this topic](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users) for instructions on how to bulk apply licenses to your users.</span></span>

- <span data-ttu-id="cdf15-108">Office ๓๖๕ผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบความปลอดภัยสามารถเข้าถึงคุณลักษณะของ Office ๓๖๕ ATP ในศูนย์\*\*\*\* \> \*\*\*\* การปฏิบัติตามกฎระเบียบความปลอดภัย _ amp_</span><span class="sxs-lookup"><span data-stu-id="cdf15-108">Office 365 global administrators or security administrators can access Office 365 ATP features in the Security & Compliance Center at **Threat Managmeent** \> **Policy**.</span></span>

- <span data-ttu-id="cdf15-109">สิ่งที่แนบมาอย่างปลอดภัยและนโยบายการเชื่อมโยงที่ปลอดภัยสามารถขอบเขตคุณทั้งองค์กรโดเมนที่เฉพาะเจาะจงหรือกลุ่มผู้ใช้ที่มีขนาดเล็กกว่า</span><span class="sxs-lookup"><span data-stu-id="cdf15-109">Safe Attachments and Safe Link policies can be scoped you your entire organization, specific domains, or smaller groups of users.</span></span>

- <span data-ttu-id="cdf15-110">ไม่มีนโยบายการแนบ ATP ที่ปลอดภัยค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="cdf15-110">There is no default ATP Safe Attachment policy.</span></span> <span data-ttu-id="cdf15-111">คุณต้อง[สร้างนโยบาย](https://docs.microsoft.com/office365/securitycompliance/set-up-atp-safe-attachments-policies)และนำไปใช้กับผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="cdf15-111">You need to [create a policy](https://docs.microsoft.com/office365/securitycompliance/set-up-atp-safe-attachments-policies) and apply it to your users.</span></span>

- <span data-ttu-id="cdf15-112">มีนโยบายการเชื่อมโยงของ ATP Safe เริ่มต้นที่ใช้กับทุกคนในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="cdf15-112">There is a default ATP Safe Links policy that applies to everyone in your organization.</span></span> <span data-ttu-id="cdf15-113">หากต้องการแก้ไขนโยบายนี้หรือสร้างนโยบายที่กำหนดเองให้ดูที่[หัวข้อนี้](https://docs.microsoft.com/office365/securitycompliance/set-up-atp-safe-links-policies)</span><span class="sxs-lookup"><span data-stu-id="cdf15-113">To edit this policy or to create custom policies, see [this topic](https://docs.microsoft.com/office365/securitycompliance/set-up-atp-safe-links-policies).</span></span>
