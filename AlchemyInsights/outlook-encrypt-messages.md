---
title: S/MIME ใน Outlook บนเว็บ
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772317"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="2b4f7-102">การเข้ารหัสลับข้อความอีเมลใน Outlook</span><span class="sxs-lookup"><span data-stu-id="2b4f7-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="2b4f7-103">การเข้ารหัสลับข้อความ microsoft ๓๖๕ถูกสร้างขึ้นบน Microsoft Azure Rights Management (Azure RMS) ซึ่งเป็นส่วนหนึ่งของการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="2b4f7-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="2b4f7-104">ถ้าการสมัครใช้งานของคุณมีการจัดการสิทธิ์ Azure หรือการป้องกันข้อมูล Azure **คุณไม่จำเป็นต้องดำเนินการใดๆในการเปิดใช้งานหรือเปิด** ใช้งานบริการการจัดการสิทธิ์ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="2b4f7-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="2b4f7-105">โดยยึดตามคำติชมของลูกค้าเราจะไม่เปิดใช้งานกฎการไหลของ Exchange mail อีกต่อไปเพื่อเข้ารหัสลับอีเมลขาออกโดยอัตโนมัติที่มีข้อมูลที่สำคัญบางชนิดในผู้เช่าของคุณตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="2b4f7-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="2b4f7-106">เราจะให้คำแนะนำโดยละเอียดเกี่ยวกับวิธีที่คุณสามารถทำได้</span><span class="sxs-lookup"><span data-stu-id="2b4f7-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="2b4f7-107">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับวิธีการสร้างกฎการขนส่งเพื่อเข้ารหัสลับข้อมูลที่สำคัญให้ดู[บทความนี้](https://aka.ms/OmeEtr)</span><span class="sxs-lookup"><span data-stu-id="2b4f7-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="2b4f7-108">ถ้าใช้ Outlook บนเว็บ (ชื่อเดิมคือ **OWA**): เมื่อเขียนข้อความอีเมลเพียงแค่คลิก **ป้องกัน** ใน OWA</span><span class="sxs-lookup"><span data-stu-id="2b4f7-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="2b4f7-109">การดำเนินการนี้จะใช้สิทธิ์ "ไม่ส่งต่อ"</span><span class="sxs-lookup"><span data-stu-id="2b4f7-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="2b4f7-110">คลิก **เปลี่ยนแปลงสิทธิ์** แล้วเลือก **เข้ารหัสลับ** เฉพาะข้อความที่เข้ารหัสลับ</span><span class="sxs-lookup"><span data-stu-id="2b4f7-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="2b4f7-111">ถ้าใช้**ไคลเอ็นต์ Outlook**: เมื่อต้องการส่งข้อความที่เข้ารหัสลับจาก outlook ๒๐๑๓หรือ๒๐๑๖หรือ Outlook ๒๐๑๖ for Mac ให้เลือกสิทธิ์**ตัวเลือก**  >  **Permissions**จากนั้นเลือกตัวเลือกการป้องกันที่คุณต้องการ</span><span class="sxs-lookup"><span data-stu-id="2b4f7-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="2b4f7-112">เมื่อต้องการ **เข้ารหัสลับอีเมลทั้งหมด** ที่ส่งไปยังผู้รับบางรายหรือองค์กรคู่ค้าภายนอกโดยอัตโนมัติคุณจำเป็นต้องสร้างกฎการขนส่งจดหมายเวียนในศูนย์การจัดการ Exchange</span><span class="sxs-lookup"><span data-stu-id="2b4f7-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="2b4f7-113">คำแนะนำโดยละเอียดจะมีให้ใน[บทความสนับสนุนนี้](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)</span><span class="sxs-lookup"><span data-stu-id="2b4f7-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

