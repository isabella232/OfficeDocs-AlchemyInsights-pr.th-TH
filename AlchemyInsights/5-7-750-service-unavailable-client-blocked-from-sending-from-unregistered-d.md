---
title: 1048 5.7.750 ไคลเอ็นต์ถูกบล็อกไม่ให้ส่งจากโดเมนที่ไม่ได้จดทะเบียน
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 48b9c2de27f8d7f52215c3a3d547bdf746a3a4cd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676732"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="b55fd-103">5.7.750 ลูกค้าถูกบล็อกไม่ให้ส่งจากโดเมนที่ไม่ได้จดทะเบียน</span><span class="sxs-lookup"><span data-stu-id="b55fd-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="b55fd-104">ข้อผิดพลาดเกิดขึ้นเมื่อมีการส่งข้อความจํานวนมากจากโดเมนที่ไม่ได้เตรียมใช้งานในผู้เช่าของคุณ (เพิ่มเป็นโดเมนที่ยอมรับและการตรวจสอบ)</span><span class="sxs-lookup"><span data-stu-id="b55fd-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="b55fd-105">เพื่อหลีกเลี่ยงข้อผิดพลาดนี้ คุณสามารถใช้ตัวเชื่อมต่อรับส่งจดหมายตามใบรับรองที่โดเมนของใบรับรองเป็นโดเมนที่เตรียมใช้งาน หรือคุณสามารถเตรียมใช้งานโดเมนที่ส่งทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="b55fd-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
