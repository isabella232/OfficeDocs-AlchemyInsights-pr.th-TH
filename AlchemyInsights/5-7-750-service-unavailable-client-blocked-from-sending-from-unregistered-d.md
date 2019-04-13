---
title: 1048 5.7.750 บริการไม่พร้อมใช้งาน ไคลเอนต์ที่ถูกบล็อกไม่ให้ส่งมาจากโดเมนที่ไม่ได้ลงทะเบียน
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 06be6babc524ae0d8065355218426c695f49be66
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/13/2019
ms.locfileid: "31856639"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="1400c-103">5.7.750 ไคลเอนต์ถูกบล็อกไม่ให้ส่งมาจากโดเมนที่ไม่ได้ลงทะเบียน</span><span class="sxs-lookup"><span data-stu-id="1400c-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="1400c-104">ข้อผิดพลาดเกิดขึ้นเมื่อขนาดใหญ่ปริมาตรของข้อความจะถูกส่งจากโดเมนที่ไม่ได้เตรียมใช้งานใน Office 365 (เพิ่มเป็นโดเมนที่ยอมรับได้ และผ่านการตรวจสอบ)</span><span class="sxs-lookup"><span data-stu-id="1400c-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="1400c-105">เมื่อต้องการหลีกเลี่ยงข้อผิดพลาดนี้ คุณสามารถใช้การเชื่อมต่อขั้นตอนอีเมลแบบผ่านการรับรองที่โดเมนใบรับรองคือ โดเมนที่เตรียมใช้งาน หรือคุณสามารถเตรียมใช้งานโดเมนทั้งหมดที่ส่ง</span><span class="sxs-lookup"><span data-stu-id="1400c-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
