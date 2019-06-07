---
title: 1048 5.7.750 บริการไม่พร้อมใช้งาน ไคลเอนต์ที่ถูกบล็อกไม่ให้ส่งมาจากโดเมนที่ไม่ได้ลงทะเบียน
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 9417fef2584e9b81a2ca71cbcc5e23ce093d94e8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34751722"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="2568e-103">5.7.750 ไคลเอนต์ถูกบล็อกไม่ให้ส่งมาจากโดเมนที่ไม่ได้ลงทะเบียน</span><span class="sxs-lookup"><span data-stu-id="2568e-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="2568e-104">ข้อผิดพลาดเกิดขึ้นเมื่อขนาดใหญ่ปริมาตรของข้อความจะถูกส่งจากโดเมนที่ไม่ได้เตรียมใช้งานใน Office 365 (เพิ่มเป็นโดเมนที่ยอมรับได้ และผ่านการตรวจสอบ)</span><span class="sxs-lookup"><span data-stu-id="2568e-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="2568e-105">เมื่อต้องการหลีกเลี่ยงข้อผิดพลาดนี้ คุณสามารถใช้การเชื่อมต่อขั้นตอนอีเมลแบบผ่านการรับรองที่โดเมนใบรับรองคือ โดเมนที่เตรียมใช้งาน หรือคุณสามารถเตรียมใช้งานโดเมนทั้งหมดที่ส่ง</span><span class="sxs-lookup"><span data-stu-id="2568e-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
