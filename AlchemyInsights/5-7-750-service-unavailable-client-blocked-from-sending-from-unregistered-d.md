---
title: บริการ 1048 5.7.750 ไม่พร้อมใช้งาน ไคลเอ็นต์ที่ถูกบล็อกจากการส่งจากโดเมนที่ไม่ได้ลงทะเบียน
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774270"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="945d6-103">5.7.750 Client ถูกบล็อกไม่ให้ส่งจากโดเมนที่ไม่ได้ลงทะเบียน</span><span class="sxs-lookup"><span data-stu-id="945d6-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="945d6-104">ข้อผิดพลาดเกิดขึ้นเมื่อข้อความปริมาณมากถูกส่งจากโดเมนที่ไม่ได้เตรียมใช้งานในผู้เช่าของคุณ (เพิ่มเป็นโดเมนที่ยอมรับและตรวจสอบความถูกต้อง)</span><span class="sxs-lookup"><span data-stu-id="945d6-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="945d6-105">เพื่อหลีกเลี่ยงข้อผิดพลาดนี้ คุณสามารถใช้ตัวเชื่อมต่อโฟลว์จดหมายที่ใช้ใบรับรองที่โดเมนของใบรับรองเป็นโดเมนที่เตรียมใช้งานแล้ว หรือคุณสามารถเตรียมใช้งานโดเมนการส่งทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="945d6-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>

<span data-ttu-id="945d6-106">For more information, see [Fix email delivery issues for error codes 5.7.700 through 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span><span class="sxs-lookup"><span data-stu-id="945d6-106">For more information, see [Fix email delivery issues for error codes 5.7.700 through 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span></span>