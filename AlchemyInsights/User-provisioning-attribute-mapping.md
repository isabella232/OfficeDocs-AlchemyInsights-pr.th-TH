---
title: การแมปแอตทริบิวต์การเตรียมใช้งานผู้ใช้
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
ms.openlocfilehash: 73da476cc5913a16911839a59b80959d3c99a8bc22471febe421b022ce2c49ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918162"
---
# <a name="user-provisioning-attribute-mapping"></a>การแมปแอตทริบิวต์การเตรียมใช้งานผู้ใช้

1. To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) ให้การสนับสนุนการเตรียมใช้งานผู้ใช้ไปยังแอปพลิเคชัน SaaS ของบริษัทอื่น เช่น Salesforce, G Suite และอื่นๆ ถ้าคุณเปิดใช้งานการเตรียมใช้งานผู้ใช้แอปพลิเคชัน SaaS ของบริษัทอื่น พอร์ทัล Azure จะควบคุมค่าแอตทริบิวต์ผ่านการแมปแอตทริบิวต์ เมื่อต้องการเรียนรู้วิธีการปรับแต่งการแมปแอตทริบิวต์เริ่มต้น ให้ดู ปรับแต่งการแมปแอตทริบิวต์การเตรียมใช้งานของผู้ใช้กับ[แอปพลิเคชัน SaaS Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)
    - เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการเตรียมใช้งานผู้ใช้แอป SaaS [ให้ดู การเตรียมใช้งานผู้ใช้แอป SaaS อัตโนมัติใน Azure AD คืออะไร](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list. ซิงค์ [แอตทริบิวต์จาก Active Directory ภายใน](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) องค์กรของคุณไปยัง Azure AD เพื่อเตรียมใช้งานบทความแอปพลิเคชันจะแสดงวิธีการเพิ่มแอตทริบิวต์ที่หายไปโดยการซิงโครไนซ์จาก AD ภายในองค์กรของคุณกับ Azure AD
