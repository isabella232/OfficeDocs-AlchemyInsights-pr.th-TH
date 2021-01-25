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
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="5f4af-102">การแมปแอตทริบิวต์การเตรียมใช้งานของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="5f4af-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="5f4af-103">เมื่อต้องการแก้ไขปัญหาการแมปแอตทริบิวต์ที่รู้จักให้ดูที่การ[แมปแอตทริบิวต์](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings)</span><span class="sxs-lookup"><span data-stu-id="5f4af-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="5f4af-104">Microsoft Azure Active Directory (AD) ให้การสนับสนุนสำหรับการเตรียมใช้งานของผู้ใช้ไปยังแอปพลิเคชัน SaaS ของบริษัทอื่นเช่น Salesforce, G Suite และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="5f4af-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="5f4af-105">ถ้าคุณเปิดใช้งานการเตรียมใช้งานของผู้ใช้สำหรับแอปพลิเคชัน SaaS ของบริษัทอื่นพอร์ทัล Azure จะควบคุมค่าแอตทริบิวต์ผ่านแอตทริบิวต์การแมป</span><span class="sxs-lookup"><span data-stu-id="5f4af-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="5f4af-106">เมื่อต้องการเรียนรู้วิธีการกำหนดค่าการแมปแอตทริบิวต์เริ่มต้นด้วยตนเองให้ดูที่[กำหนดแอตทริบิวต์การเตรียมใช้งานของผู้ใช้เอง-แมปสำหรับแอปพลิเคชัน SaaS ใน Azure Active directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)</span><span class="sxs-lookup"><span data-stu-id="5f4af-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="5f4af-107">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการเตรียมใช้งานแอป SaaS ให้ดู [ที่การเตรียมใช้งานผู้ใช้แอป saas อัตโนมัติใน AZURE AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="5f4af-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="5f4af-108">เมื่อกำหนดแอตทริบิวต์เอง-การแมปสำหรับการเตรียมใช้งานของผู้ใช้คุณอาจพบว่าแอตทริบิวต์ที่คุณต้องการแมปไม่ปรากฏในรายการแอตทริบิวต์ต้นฉบับ</span><span class="sxs-lookup"><span data-stu-id="5f4af-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="5f4af-109">การ [ซิงค์แอตทริบิวต์จาก Active directory ภายในองค์กรของคุณไปยัง AZURE AD สำหรับการเตรียมใช้งานบทความแอปพลิเคชันแสดงให้](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) คุณเห็นวิธีการเพิ่มแอตทริบิวต์ที่ขาดหายไปโดยการซิงโครไนซ์จากโฆษณาภายในองค์กรของคุณไปยัง azure ad</span><span class="sxs-lookup"><span data-stu-id="5f4af-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
