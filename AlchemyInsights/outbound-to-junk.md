---
title: อีเมลขาออกไปยังโฟลเดอร์อีเมลขยะ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 2350586e95f316061ff855d152e86db0547eb209
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761187"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="4c348-102">อีเมลขาออกไปยังโฟลเดอร์อีเมลขยะ</span><span class="sxs-lookup"><span data-stu-id="4c348-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="4c348-103">หากคุณเห็นข้อความขาออกถูกทําเครื่องหมายว่าเป็นขยะ ให้ทําตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="4c348-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="4c348-104">หากคุณยังไม่ได้กําหนดค่า[การแจ้งเตือนนโยบายสแปมขาออก](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy)</span><span class="sxs-lookup"><span data-stu-id="4c348-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="4c348-105">ใช้[การติดตามข้อความ](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc)เพื่อดูว่าข้อความขาออกมีค่าเหตุการณ์**สแปม**ที่มีรายละเอียดเพิ่มเติมหรือไม่:**ใช้กลุ่มการจัดส่งที่มีความเสี่ยงสูง**</span><span class="sxs-lookup"><span data-stu-id="4c348-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="4c348-106">สําหรับข้อความเหล่านี้ ให้ตรวจสอบเนื้อหาข้อความเพื่อดูว่าอาจเป็นสแปม</span><span class="sxs-lookup"><span data-stu-id="4c348-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="4c348-107">ตัวอย่างเช่น ลายเซ็นบางครั้งอาจทําให้เกิดปัญหาสําหรับผู้ใช้จํานวนมาก</span><span class="sxs-lookup"><span data-stu-id="4c348-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="4c348-108">หากคุณมีหลายตัวอย่างของข้อความขาออกที่ถูกต้องที่ถูกทําเครื่องหมายว่าเป็นขยะให้เปิดตั๋วสนับสนุนและขอให้ตัวแทนฝ่ายสนับสนุนส่งข้อความของคุณเป็นบวกปลอมไปยังนักวิเคราะห์สแปมของเรา</span><span class="sxs-lookup"><span data-stu-id="4c348-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="4c348-109">เตรียมการจัดเตรียมข้อความตัวอย่างที่มีส่วนหัวของข้อความทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="4c348-109">Be prepared to provide sample messages that include all message headers.</span></span>
