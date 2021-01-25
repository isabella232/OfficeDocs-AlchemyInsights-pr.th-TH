---
title: การแมปแอตทริบิวต์การเตรียมใช้งานของผู้ใช้
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949898"
---
# <a name="user-provisioning-attribute-mapping"></a>การแมปแอตทริบิวต์การเตรียมใช้งานของผู้ใช้

1. เมื่อต้องการแก้ไขปัญหาการแมปแอตทริบิวต์ที่รู้จักให้ดูที่การ[แมปแอตทริบิวต์](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings) 
2. Microsoft Azure Active Directory (AD) ให้การสนับสนุนสำหรับการเตรียมใช้งานของผู้ใช้ไปยังแอปพลิเคชัน SaaS ของบริษัทอื่นเช่น Salesforce, G Suite และอื่นๆ ถ้าคุณเปิดใช้งานการเตรียมใช้งานของผู้ใช้สำหรับแอปพลิเคชัน SaaS ของบริษัทอื่นพอร์ทัล Azure จะควบคุมค่าแอตทริบิวต์ผ่านแอตทริบิวต์การแมป เมื่อต้องการเรียนรู้วิธีการกำหนดค่าการแมปแอตทริบิวต์เริ่มต้นด้วยตนเองให้ดูที่[กำหนดแอตทริบิวต์การเตรียมใช้งานของผู้ใช้เอง-แมปสำหรับแอปพลิเคชัน SaaS ใน Azure Active directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)
    - เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการเตรียมใช้งานแอป SaaS ให้ดู [ที่การเตรียมใช้งานผู้ใช้แอป saas อัตโนมัติใน AZURE AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. เมื่อกำหนดแอตทริบิวต์เอง-การแมปสำหรับการเตรียมใช้งานของผู้ใช้คุณอาจพบว่าแอตทริบิวต์ที่คุณต้องการแมปไม่ปรากฏในรายการแอตทริบิวต์ต้นฉบับ การ [ซิงค์แอตทริบิวต์จาก Active directory ภายในองค์กรของคุณไปยัง AZURE AD สำหรับการเตรียมใช้งานบทความแอปพลิเคชันแสดงให้](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) คุณเห็นวิธีการเพิ่มแอตทริบิวต์ที่ขาดหายไปโดยการซิงโครไนซ์จากโฆษณาภายในองค์กรของคุณไปยัง azure ad
