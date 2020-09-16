---
title: อีเมลขาออกไปยังโฟลเดอร์อีเมลขยะ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769202"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="a34e3-102">อีเมลขาออกไปยังโฟลเดอร์อีเมลขยะ</span><span class="sxs-lookup"><span data-stu-id="a34e3-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="a34e3-103">ถ้าคุณเห็นข้อความขาออกที่ถูกทำเครื่องหมายเป็นอีเมลขยะให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a34e3-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="a34e3-104">ถ้าคุณยังไม่ได้ทำให้ลอง[กำหนดค่าการแจ้งให้ทราบเกี่ยวกับนโยบายสแปมขาออก](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)</span><span class="sxs-lookup"><span data-stu-id="a34e3-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="a34e3-105">ใช้การ[ติดตามข้อความ](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc)เพื่อดูว่าข้อความขาออกมีค่าอี**เมลสแปม**ที่มีรายละเอียดเพิ่มเติมหรือไม่ให้**ใช้กลุ่มการจัดส่งที่มีความเสี่ยงสูง**</span><span class="sxs-lookup"><span data-stu-id="a34e3-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="a34e3-106">สำหรับข้อความเหล่านี้ให้ตรวจสอบเนื้อหาข้อความเพื่อดูสิ่งที่อาจถือว่าเป็นสแปม</span><span class="sxs-lookup"><span data-stu-id="a34e3-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="a34e3-107">ตัวอย่างเช่นลายเซ็นบางครั้งอาจทำให้เกิดปัญหาสำหรับผู้ใช้หลายคน</span><span class="sxs-lookup"><span data-stu-id="a34e3-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="a34e3-108">ถ้าคุณมีหลายตัวอย่างของข้อความขาออกที่ถูกทำเครื่องหมายว่าเป็นอีเมลขยะให้เปิดบัตรสนับสนุนและขอให้เจ้าหน้าที่สนับสนุนส่งข้อความของคุณเป็น false บวกไปถึงนักวิเคราะห์สแปมของเรา</span><span class="sxs-lookup"><span data-stu-id="a34e3-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="a34e3-109">เตรียมพร้อมที่จะให้ข้อความตัวอย่างที่มีส่วนหัวของข้อความทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="a34e3-109">Be prepared to provide sample messages that include all message headers.</span></span>
