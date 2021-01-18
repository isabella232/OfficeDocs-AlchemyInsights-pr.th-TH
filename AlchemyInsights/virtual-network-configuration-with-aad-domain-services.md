---
title: การกำหนดค่าเสมือนกับบริการโดเมน AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885652"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>การกำหนดค่าเสมือนกับบริการโดเมน AAD

การกำหนดค่าเสมือนกับบริการโดเมน AAD มีขั้นตอนต่อไปนี้: 

1. การตรวจสอบสถานภาพโดเมนของคุณบนพอร์ทัล Azure https://aka.ms/aadds-health
2. การตรวจสอบการ NSG ของคุณสำหรับกฎที่บล็อกพอร์ตที่จำเป็นในการซิงโครไนซ์ในบริการโดเมน AD Azure บนพอร์ทัล https://aka.ms/aadds-networking
3. ตรวจสอบให้แน่ใจว่าเครือข่ายเสมือนของคุณได้รับการปรับใช้ในภูมิภาค Azure เดียวกันกับโดเมนที่มีการจัดการบริการ Domain AD Azure ของคุณ
4. ตรวจสอบให้แน่ใจว่าคุณไม่มีโดเมนที่มีอยู่ที่มีชื่อโดเมนเดียวกันกับที่มีอยู่บนเครือข่ายเสมือน

สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับการพิจารณาการออกแบบบนเครือข่ายเสมือนของ Azure เพื่อสนับสนุนบริการ domain domain ให้ดูที่การ[พิจารณาเครือข่ายเสมือน](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)

