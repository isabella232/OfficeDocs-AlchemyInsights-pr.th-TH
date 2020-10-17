---
title: ๗๒๖การบล็อกการส่งต่ออีเมล
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473120"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="fa6a4-102">การบล็อกหรือการยกเลิกการบล็อกการส่งต่ออีเมล</span><span class="sxs-lookup"><span data-stu-id="fa6a4-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="fa6a4-103">เมื่อต้องการเปิดหรือปิดใช้งานการส่งต่ออีเมลสำหรับกล่องจดหมายที่เฉพาะเจาะจงให้ดูที่[กำหนดค่าการส่งต่ออีเมล](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)</span><span class="sxs-lookup"><span data-stu-id="fa6a4-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="fa6a4-104">ในระดับผู้เช่าการควบคุมการส่งต่อภายนอกจะเสร็จสมบูรณ์โดยใช้นโยบายสแปมขาออก</span><span class="sxs-lookup"><span data-stu-id="fa6a4-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="fa6a4-105">คุณสามารถตรวจสอบนโยบายตัวกรองสแปมขาออกจากศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย [ต่อไปนี้] ( https://protection.office.com/antispam) หรือโดยใช้[คำสั่ง Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)</span><span class="sxs-lookup"><span data-stu-id="fa6a4-105">You can check the outbound spam filter policy from Security and Compliance Center [here] (https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="fa6a4-106">ถ้าคุณได้รับข้อผิดพลาดต่อไปนี้: **"๕๕๐ 5.7.520 Access ถูกปฏิเสธองค์กรของคุณไม่อนุญาตให้มีการส่งต่อภายนอก"** โปรดตรวจสอบให้แน่ใจว่านโยบายถูกกำหนดค่าให้เปิดใช้งานการส่งต่อภายนอกโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="fa6a4-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="fa6a4-107">**หมายเหตุ:** ขอแนะนำให้ทำการปิดใช้งาน Autoforward ภายนอกในนโยบายตัวกรองสแปมขาออกเริ่มต้นของคุณและเปิดใช้งานเฉพาะสำหรับผู้ใช้ที่ต้องการการส่งต่อภายนอกโดยการสร้างนโยบายแบบกำหนดเองสำหรับผู้ใช้เหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="fa6a4-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="fa6a4-108">คุณสามารถอ่านเพิ่มเติมได้ในการ[กำหนดค่าการส่งต่ออีเมลภายนอกใน Office ๓๖๕](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)</span><span class="sxs-lookup"><span data-stu-id="fa6a4-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>