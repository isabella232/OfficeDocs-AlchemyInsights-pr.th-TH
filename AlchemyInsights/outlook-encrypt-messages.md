---
title: S/MIME ใน Outlook บนเว็บ
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666859"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="4b5ea-102">เข้ารหัสข้อความทางเมลใน Outlook</span><span class="sxs-lookup"><span data-stu-id="4b5ea-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="4b5ea-103">การเข้ารหัสลับข้อความของ Office ๓๖๕ถูกสร้างขึ้นบน Microsoft Azure สิทธิ์การจัดการ (Azure RMS) ซึ่งเป็นส่วนหนึ่งของการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="4b5ea-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="4b5ea-104">ถ้าการสมัครสมาชิกของคุณมีการจัดการสิทธิ์ Azure หรือการป้องกันข้อมูล Azure**คุณไม่จำเป็นต้องดำเนินการใดๆเพื่อเปิดใช้งานหรือเปิดใช้**งานบริการการจัดการสิทธิ์ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="4b5ea-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="4b5ea-105">ขึ้นอยู่กับความคิดเห็นของลูกค้าเราจะไม่เปิดใช้งานกฎการไหลของจดหมาย Exchange เพื่อเข้ารหัสลับโดยอัตโนมัติที่มีบางชนิดของข้อมูลที่สำคัญในผู้เช่าของคุณโดยค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="4b5ea-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="4b5ea-106">แต่เราจะให้คำแนะนำโดยละเอียดเกี่ยวกับวิธีการที่คุณสามารถทำได้ด้วยตัวเอง</span><span class="sxs-lookup"><span data-stu-id="4b5ea-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="4b5ea-107">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับวิธีการสร้างกฎการขนส่งเพื่อเข้ารหัสลับข้อมูลที่สำคัญโปรดดู[บทความนี้](https://aka.ms/OmeEtr)</span><span class="sxs-lookup"><span data-stu-id="4b5ea-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="4b5ea-108">ถ้าใช้ Outlook บนเว็บ (เดิมคือ**OWA**): เมื่อเขียนข้อความทาง e-mail เพียงแค่คลิก**ป้องกัน**ใน OWA</span><span class="sxs-lookup"><span data-stu-id="4b5ea-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="4b5ea-109">การดำเนินการนี้จะใช้ "อย่าส่งต่อ" ได้รับอนุญาต</span><span class="sxs-lookup"><span data-stu-id="4b5ea-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="4b5ea-110">คลิ**กเปลี่ยนแปลงสิทธิ์**และเลือกเข้า**รหัส**เพื่อเข้ารหัสข้อความเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="4b5ea-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="4b5ea-111">ถ้าใช้**ไคลเอนต์ outlook**: เมื่อต้องการส่งข้อความที่เข้ารหัสลับจาก outlook ๒๐๑๓หรือ๒๐๑๖หรือ Outlook ๒๐๑๖สำหรับ Mac ให้เลือก**สิทธิ์\*\*\*\*ตัวเลือก** > จากนั้นเลือกตัวเลือกการป้องกันที่คุณต้องการ</span><span class="sxs-lookup"><span data-stu-id="4b5ea-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="4b5ea-112">หากต้องการเข้า**รหัสลับทั้งหมด**ที่ส่งไปยังผู้รับบางรายหรือองค์กรหุ้นส่วนภายนอกโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="4b5ea-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="4b5ea-113">คำแนะนำโดยละเอียดจะมีให้ใน[บทความสนับสนุนนี้](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)</span><span class="sxs-lookup"><span data-stu-id="4b5ea-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

