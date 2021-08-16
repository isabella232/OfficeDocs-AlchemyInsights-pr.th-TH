---
title: การกําหนดค่าเสมือนด้วยบริการโดเมน AAD
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
ms.openlocfilehash: 03a6ec63ba8e2779b0fe3f0381606af2c0748f8b848baaa7cd88b61317bd7a5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072863"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>การกําหนดค่าเสมือนด้วยบริการโดเมน AAD

การกําหนดค่าเสมือนกับบริการโดเมน AAD เกี่ยวข้องกับขั้นตอนต่อไปนี้: 

1. การตรวจสอบสถานภาพโดเมนของคุณบนพอร์ทัล Azure https://aka.ms/aadds-health
2. การตรวจสอบกฎ NSG ของคุณที่บล็อกพอร์ตที่ต้องใช้ในการซิงโครไนซ์ใน Azure AD Domain Services บนพอร์ทัล https://aka.ms/aadds-networking
3. ตรวจสอบว่าเครือข่ายเสมือนของคุณถูกปรับใช้ในภูมิภาค Azure เดียวกันกับโดเมน Azure AD Domain Services ที่มีการจัดการ
4. ตรวจสอบว่าคุณไม่มีโดเมนที่มีอยู่แล้วที่มีชื่อโดเมนเดียวกันที่พร้อมใช้งานบนเครือข่ายเสมือน

For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

