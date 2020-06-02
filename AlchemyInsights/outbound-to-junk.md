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
ms.openlocfilehash: 869cd3d9fb8e5fce291244e4a39754d074b11358
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511743"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="6886f-102">อีเมลขาออกไปยังโฟลเดอร์อีเมลขยะ</span><span class="sxs-lookup"><span data-stu-id="6886f-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="6886f-103">หากคุณเห็นข้อความขาออกถูกทําเครื่องหมายเป็นอีเมลขยะ ให้ทําตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="6886f-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="6886f-104">หากคุณยังไม่ได้พิจารณา[การกําหนดค่าการแจ้งเตือนนโยบายสแปมขาออก](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)</span><span class="sxs-lookup"><span data-stu-id="6886f-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="6886f-105">ใช้[การติดตามข้อความ](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc)เพื่อดูว่าข้อความขาออกมีค่าเหตุการณ์**เป็นสแปม**ที่มีรายละเอียดเพิ่มเติมหรือไม่:**ใช้พูลการรับสินค้าที่มีความเสี่ยงสูง**</span><span class="sxs-lookup"><span data-stu-id="6886f-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="6886f-106">สําหรับข้อความเหล่านี้ ให้ตรวจสอบเนื้อหาข้อความเพื่อดูว่าสแปมใด</span><span class="sxs-lookup"><span data-stu-id="6886f-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="6886f-107">ตัวอย่างเช่น ลายเซ็นบางครั้งอาจทําให้เกิดปัญหาสําหรับผู้ใช้หลายคน</span><span class="sxs-lookup"><span data-stu-id="6886f-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="6886f-108">หากคุณมีตัวอย่างข้อความขาออกที่ถูกต้องหลายข้อที่ถูกทําเครื่องหมายว่าเป็น Junk ให้เปิดตั๋วสนับสนุนและขอให้ตัวแทนฝ่ายสนับสนุนส่งข้อความของคุณเป็นข้อมูลบวกปลอมให้กับนักวิเคราะห์สแปมของเรา</span><span class="sxs-lookup"><span data-stu-id="6886f-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="6886f-109">เตรียมข้อความตัวอย่างที่มีส่วนหัวของข้อความทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="6886f-109">Be prepared to provide sample messages that include all message headers.</span></span>
