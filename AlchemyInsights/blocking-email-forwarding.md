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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219874"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="9a625-102">การบล็อกหรือการยกเลิกการบล็อกการส่งต่ออีเมล</span><span class="sxs-lookup"><span data-stu-id="9a625-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="9a625-103">เมื่อต้องการเปิดหรือปิดใช้งานการส่งต่ออีเมลสำหรับกล่องจดหมายที่เฉพาะเจาะจงให้ดูที่[กำหนดค่าการส่งต่ออีเมล](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)</span><span class="sxs-lookup"><span data-stu-id="9a625-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="9a625-104">ในระดับผู้เช่าการควบคุมการส่งต่อภายนอกจะเสร็จสมบูรณ์โดยใช้นโยบายการป้องกันสแปมขาออก</span><span class="sxs-lookup"><span data-stu-id="9a625-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="9a625-105">ถ้าถูกตั้งค่าเป็นปิดหรืออัตโนมัติอาจเป็นการบล็อกการส่งต่ออีเมลด้วยข้อผิดพลาด "๕๕๐ 5.7.520 Access ถูกปฏิเสธองค์กรของคุณไม่อนุญาตให้มีการส่งต่อภายนอก"</span><span class="sxs-lookup"><span data-stu-id="9a625-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="9a625-106">ในภายหลังถ้าการส่งต่อถูกตั้งค่าให้ถูกบล็อกนั่นเป็นข้อผิดพลาดที่ผู้ใช้ของคุณจะเห็น</span><span class="sxs-lookup"><span data-stu-id="9a625-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="9a625-107">ถ้าการส่งต่อถูกบล็อกโปรดตรวจสอบให้แน่ใจว่าได้กำหนดค่านโยบายให้เปิดใช้งาน Autoforward ภายนอก</span><span class="sxs-lookup"><span data-stu-id="9a625-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="9a625-108">คุณสามารถตรวจสอบนโยบายตัวกรองสแปมขาออกจากศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายหรือโดยการเรียกใช้คำสั่ง HostedOutboundSpamFilterPolicy | ชื่อ fl, AutoForwardingMode</span><span class="sxs-lookup"><span data-stu-id="9a625-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="9a625-109">ถ้าคุณต้องการตั้งค่าการบล็อก Autoforward คำสั่งเดียวกันจะบอกสถานะของนโยบายในตอนนี้</span><span class="sxs-lookup"><span data-stu-id="9a625-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="9a625-110">หมายเหตุ: ขอแนะนำให้ปิดใช้งาน Autoforward ภายนอกในนโยบายตัวกรองสแปมขาออกเริ่มต้นของคุณและเปิดใช้งานสำหรับผู้ใช้ที่ต้องการการส่งต่อภายนอกโดยการสร้างนโยบายแบบกำหนดเองสำหรับผู้ใช้เหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="9a625-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="9a625-111">คุณสามารถอ่านเพิ่มเติมได้ในการ[กำหนดค่าการส่งต่ออีเมลภายนอกใน Office ๓๖๕](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)</span><span class="sxs-lookup"><span data-stu-id="9a625-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>