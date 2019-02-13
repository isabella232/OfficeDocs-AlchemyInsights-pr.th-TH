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
ms.openlocfilehash: 5fe5b343d89c49e1805e4d0cac6698ef35e1dd30
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921943"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="484a8-103">5.7.750 ไคลเอนต์ถูกบล็อกไม่ให้ส่งมาจากโดเมนที่ไม่ได้ลงทะเบียน</span><span class="sxs-lookup"><span data-stu-id="484a8-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="484a8-104">ข้อผิดพลาดเกิดขึ้นเมื่อขนาดใหญ่ปริมาตรของข้อความจะถูกส่งจากโดเมนที่ไม่ได้เตรียมใช้งานใน Office 365 (เพิ่มเป็นโดเมนที่ยอมรับได้ และผ่านการตรวจสอบ)</span><span class="sxs-lookup"><span data-stu-id="484a8-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>
  
<span data-ttu-id="484a8-105">เมื่อต้องการหลีกเลี่ยงข้อผิดพลาดนี้ คุณสามารถใช้การเชื่อมต่อขั้นตอนอีเมลแบบผ่านการรับรองที่โดเมนใบรับรองคือ โดเมนที่เตรียมใช้งาน หรือคุณสามารถเตรียมใช้งานโดเมนทั้งหมดที่ส่ง</span><span class="sxs-lookup"><span data-stu-id="484a8-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
  

