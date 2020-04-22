---
title: S/MIME ใน Outlook บนเว็บ
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764891"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="9e885-102">เข้ารหัสข้อความอีเมลใน Outlook</span><span class="sxs-lookup"><span data-stu-id="9e885-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="9e885-103">การเข้ารหัสลับข้อความของ Microsoft 365 สร้างขึ้นบน Microsoft Azure สิทธิ์จัดการ (Azure RMS), ซึ่งเป็นส่วนหนึ่งของการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="9e885-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="9e885-104">ถ้าการสมัครใช้งานของคุณมีการจัดการสิทธิ์ Azure หรือการป้องกันข้อมูล Azure**คุณไม่จําเป็นต้องดําเนินการใดๆ เพื่อเปิดใช้งานหรือเปิดใช้งาน**บริการการจัดการสิทธิ์ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="9e885-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="9e885-105">จากคําติชมของลูกค้า เราจะไม่เปิดใช้งานกฎการรับจดหมาย Exchange เพื่อเข้ารหัสอีเมลขาออกที่มีข้อมูลละเอียดอ่อนบางชนิดในผู้เช่าของคุณตามค่าเริ่มต้นอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="9e885-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="9e885-106">แต่เราให้คําแนะนําโดยละเอียดเกี่ยวกับวิธีที่คุณทําเช่นนั้นได้</span><span class="sxs-lookup"><span data-stu-id="9e885-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="9e885-107">สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับวิธีการสร้างกฎการส่งผ่านเพื่อเข้ารหัสลับข้อมูลที่ละเอียดอ่อน ให้ดูที่[บทความนี้](https://aka.ms/OmeEtr)</span><span class="sxs-lookup"><span data-stu-id="9e885-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="9e885-108">ถ้าใช้ Outlook บนเว็บ (เดิม**คือ OWA):** เมื่อเขียนข้อความอีเมล เพียงคลิก**ป้องกัน**ใน OWA</span><span class="sxs-lookup"><span data-stu-id="9e885-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="9e885-109">ซึ่งจะใช้สิทธิ์ "ไม่ต้องส่งต่อ"</span><span class="sxs-lookup"><span data-stu-id="9e885-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="9e885-110">คลิก**เปลี่ยนแปลงสิทธิ์**แล้วเลือก**เข้ารหัส**เพื่อเข้ารหัสลับข้อความเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="9e885-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="9e885-111">หากใช้**ไคลเอนต์ Outlook:** เมื่อต้องการส่งข้อความที่เข้ารหัสจาก Outlook 2013 หรือ 2016 หรือ Outlook 2016 for Mac ให้เลือก**สิทธิ์\*\*\*\*ตัวเลือก** > จากนั้นเลือกตัวเลือกการป้องกันที่คุณต้องการ</span><span class="sxs-lookup"><span data-stu-id="9e885-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="9e885-112">เมื่อต้องการ**เข้ารหัสลับอีเมลทั้งหมดที่**ส่งไปยังผู้รับหรือองค์กรคู่ค้าภายนอกบางแห่งโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="9e885-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="9e885-113">คําแนะนําโดยละเอียดมีให้ใน[บทความสนับสนุนนี้](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)</span><span class="sxs-lookup"><span data-stu-id="9e885-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

