---
title: บริการ๑๐๔๘5.7.750 ไม่พร้อมใช้งาน ไคลเอ็นต์ถูกบล็อกจากการส่งจากโดเมนที่ไม่ได้ลงทะเบียน
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
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664261"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="e0719-103">ไคลเอ็นต์5.7.750 ถูกบล็อกจากการส่งจากโดเมนที่ไม่ได้ลงทะเบียน</span><span class="sxs-lookup"><span data-stu-id="e0719-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="e0719-104">ข้อผิดพลาดจะเกิดขึ้นเมื่อมีการส่งข้อความจำนวนมากจากโดเมนที่ไม่ได้เตรียมใช้งานในผู้เช่าของคุณ (เพิ่มเป็นโดเมนที่ยอมรับได้และการตรวจสอบความถูกต้องของข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="e0719-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="e0719-105">เมื่อต้องการหลีกเลี่ยงข้อผิดพลาดนี้คุณสามารถใช้ตัวเชื่อมต่อเวิร์กโฟลว์จดหมายที่ใช้ใบรับรองที่โดเมนของใบรับรองเป็นโดเมน provisioned หรือคุณสามารถจัดเตรียมโดเมนการส่งทั้งหมดได้</span><span class="sxs-lookup"><span data-stu-id="e0719-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
