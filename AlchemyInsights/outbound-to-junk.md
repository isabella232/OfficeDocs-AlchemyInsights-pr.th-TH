---
title: เมลขาออกไปยังโฟลเดอร์เมลขยะ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 371d2c46e9048365fd343145330536bd9cf1db82
ms.sourcegitcommit: 1002f510fadb92c143cd6bbb60b42a851d5a38e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/20/2019
ms.locfileid: "37062852"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="8d55c-102">เมลขาออกไปยังโฟลเดอร์เมลขยะ</span><span class="sxs-lookup"><span data-stu-id="8d55c-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="8d55c-103">หากคุณเห็นข้อความขาออกที่ถูกทำเครื่องหมายว่าเป็นขยะให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="8d55c-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="8d55c-104">หากคุณยังไม่เคยลอง[กำหนดค่าการแจ้งเตือนนโยบายสแปมขาออก](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy)</span><span class="sxs-lookup"><span data-stu-id="8d55c-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="8d55c-105">ใช้การ[ติดตามข้อความ](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc)เพื่อดูว่าข้อความขาออกมีค่าเหตุการณ์**สแปม**ด้วยรายละเอียดเพิ่มเติม:**ใช้กลุ่มการส่งความเสี่ยงสูง**</span><span class="sxs-lookup"><span data-stu-id="8d55c-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="8d55c-106">สำหรับข้อความเหล่านี้ให้ตรวจสอบเนื้อหาของข้อความเพื่อดูสิ่งที่อาจถือว่าเป็นสแปม</span><span class="sxs-lookup"><span data-stu-id="8d55c-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="8d55c-107">ตัวอย่างเช่นลายเซ็นบางครั้งอาจทำให้เกิดปัญหาสำหรับผู้ใช้จำนวนมาก</span><span class="sxs-lookup"><span data-stu-id="8d55c-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="8d55c-108">หากคุณมีหลายตัวอย่างของข้อความขาออกที่ถูกต้องตามกฎหมายที่ถูกทำเครื่องหมายว่าเป็นขยะให้เปิดตั๋วสนับสนุนและขอให้ตัวแทนฝ่ายสนับสนุนส่งข้อความของคุณให้เป็นเท็จกับนักวิเคราะห์สแปมของเรา</span><span class="sxs-lookup"><span data-stu-id="8d55c-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="8d55c-109">เตรียมพร้อมที่จะให้ข้อความตัวอย่างที่มีส่วนหัวของข้อความทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="8d55c-109">Be prepared to provide sample messages that include all message headers.</span></span>
