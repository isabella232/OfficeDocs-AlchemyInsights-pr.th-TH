---
title: ลักษณะการสอดคล้องGuid / sourceAnchor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817011"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="e8b4b-102">ลักษณะการสอดคล้องGuid / sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="e8b4b-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="e8b4b-103">Azure AD Connect (เวอร์ชัน 1.1.524.0 และหลังจากนั้น) ช่วยให้การใช้ msDS-ConsistencyGuid เป็นแอตทริบิวต์ SourceAnchor ง่ายขึ้น</span><span class="sxs-lookup"><span data-stu-id="e8b4b-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="e8b4b-104">เมื่อใช้ฟีเจอร์นี้ Azure AD Connect จะกําหนดค่ากฎการซิงโครไนซ์ให้โดยอัตโนมัติ:</span><span class="sxs-lookup"><span data-stu-id="e8b4b-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="e8b4b-105">ใช้ msDS-ConsistencyGuid เป็นแอตทริบิวต์ SourceAnchor ของวัตถุผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="e8b4b-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="e8b4b-106">ObjectGUID จะถูกใช้กับวัตถุชนิดอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="e8b4b-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="e8b4b-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="e8b4b-108">หลังจากสร้างแอตทริบิวต์ msDS-ConsistencyGuid แล้ว Azure AD Connect จะส่งออกวัตถุไปยัง Azure AD</span><span class="sxs-lookup"><span data-stu-id="e8b4b-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="e8b4b-109">**หมายเหตุ:** เมื่อนําเข้าวัตถุ AD ภายในองค์กรลงใน Azure AD Connect (ซึ่งนําเข้าลงในพื้นที่ตัวเชื่อมต่อ AD และที่ฉายลงใน Metaverse) คุณจะไม่สามารถเปลี่ยนค่า SourceAnchor ของวัตถุได้อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="e8b4b-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="e8b4b-110">เมื่อต้องการระบุค่า SourceAnchor ของวัตถุ AD ภายในองค์กรที่กําหนด ให้กําหนดค่าแอตทริบิวต์ msDS-ConsistencyGuid ของวัตถุก่อนที่จะถูกนําเข้าลงใน Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e8b4b-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="e8b4b-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="e8b4b-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

