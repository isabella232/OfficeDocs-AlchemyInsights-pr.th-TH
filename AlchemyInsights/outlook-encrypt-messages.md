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
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511527"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="9902a-102">เข้ารหัสข้อความอีเมลใน Outlook</span><span class="sxs-lookup"><span data-stu-id="9902a-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="9902a-103">การเข้ารหัสลับข้อความ Microsoft 365 สร้างขึ้นบน Microsoft Azure จัดการสิทธิ์ (Azure RMS), ซึ่งเป็นส่วนหนึ่งของการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="9902a-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="9902a-104">ถ้าการสมัครใช้งานของคุณมีการจัดการสิทธิ์ Azure หรือการป้องกันข้อมูล Azure**คุณไม่จําเป็นต้องดําเนินการใดๆ เพื่อเปิดใช้งานหรือเปิดใช้งาน**บริการการจัดการสิทธิ์ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="9902a-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="9902a-105">โดยยึดตามคําติชมของลูกค้า เราจะไม่เปิดใช้งานกฎการรับส่งจดหมายของ Exchange เพื่อเข้ารหัสอีเมลขาออกที่มีข้อมูลที่สําคัญบางชนิดในผู้เช่าของคุณตามค่าเริ่มต้นอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="9902a-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="9902a-106">แต่เราจะให้คําแนะนําโดยละเอียดเกี่ยวกับวิธีที่คุณสามารถทําได้เอง</span><span class="sxs-lookup"><span data-stu-id="9902a-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="9902a-107">สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับวิธีสร้างกฎการขนส่งเพื่อเข้ารหัสลับข้อมูลสําคัญ ให้ดู[บทความนี้](https://aka.ms/OmeEtr)</span><span class="sxs-lookup"><span data-stu-id="9902a-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="9902a-108">ถ้าใช้ Outlook บนเว็บ (เดิม**คือ OWA):** เมื่อเขียนข้อความอีเมล เพียงคลิก**ป้องกัน**ใน OWA</span><span class="sxs-lookup"><span data-stu-id="9902a-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="9902a-109">นี้จะนําไปใช้ "ไม่ส่งต่อ" สิทธิ์</span><span class="sxs-lookup"><span data-stu-id="9902a-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="9902a-110">คลิก**เปลี่ยนสิทธิ์**แล้วเลือก**เข้ารหัสลับ**เพื่อเข้ารหัสเฉพาะข้อความเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="9902a-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="9902a-111">ถ้าใช้**ไคลเอ็นต์ Outlook**: เมื่อต้องการส่งข้อความที่เข้ารหัสลับจาก Outlook 2013 หรือ 2016 หรือ Outlook 2016 for Mac ให้เลือก**ตัวเลือก**  >  **สิทธิ์**จากนั้นเลือกตัวเลือกการป้องกันที่คุณต้องการ</span><span class="sxs-lookup"><span data-stu-id="9902a-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="9902a-112">เมื่อต้องการ**เข้ารหัสลับอีเมลทั้งหมดที่**ส่งไปยังผู้รับหรือองค์กรคู่ค้าภายนอกโดยอัตโนมัติ คุณจําเป็นต้องสร้างกฎการส่งจดหมายในศูนย์ดูแล Exchange</span><span class="sxs-lookup"><span data-stu-id="9902a-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="9902a-113">คําแนะนําโดยละเอียดมีให้ใน[บทความสนับสนุนนี้](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)</span><span class="sxs-lookup"><span data-stu-id="9902a-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

