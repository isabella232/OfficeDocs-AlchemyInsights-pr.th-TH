---
title: การซิงโครไนซ์บริการโดเมน
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885561"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="07b55-102">การซิงโครไนซ์บริการโดเมน</span><span class="sxs-lookup"><span data-stu-id="07b55-102">Domain service synchronization</span></span>

<span data-ttu-id="07b55-103">วัตถุและข้อมูลประจำตัวในโดเมน Azure Active Directory Services (Azure AD DS) สามารถถูกสร้างขึ้นภายในโดเมนหรือซิงโครไนซ์จากผู้เช่า Azure Active directory (Azure ad) ได้อย่างใดอย่างหนึ่ง</span><span class="sxs-lookup"><span data-stu-id="07b55-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="07b55-104">เมื่อคุณปรับใช้ Azure AD DS เป็นครั้งแรกการซิงโครไนซ์แบบครั้งเดียวโดยอัตโนมัติถูกกำหนดค่าและเริ่มต้นการทำซ้ำวัตถุจาก Azure AD</span><span class="sxs-lookup"><span data-stu-id="07b55-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="07b55-105">การซิงโครไนซ์ครั้งเดียวนี้จะยังคงทำงานในพื้นหลังเพื่อเก็บ Azure AD DS ที่มีการจัดการโดเมนที่มีการเปลี่ยนแปลงที่มีการเปลี่ยนแปลงใดๆจาก Azure AD</span><span class="sxs-lookup"><span data-stu-id="07b55-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="07b55-106">ไม่มีการซิงโครไนซ์เกิดขึ้นจาก Azure AD DS กลับไปยัง Azure AD</span><span class="sxs-lookup"><span data-stu-id="07b55-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="07b55-107">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับการซิงโครไนซ์บริการโดเมนของ Active Directory ของ Azure ให้ดูที่การ[ซิงโครไนซ์บริการโดเมน](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization)</span><span class="sxs-lookup"><span data-stu-id="07b55-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
