---
title: ลักษณะการทำงาน ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756302"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="d9630-102">ลักษณะการทำงาน ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="d9630-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="d9630-103">Azure AD Connect (เวอร์ชัน1.1.524.0 และหลังจากนี้) จะอำนวยความสะดวกในการใช้งานของ msDS-ConsistencyGuid เป็นแอตทริบิวต์ sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="d9630-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="d9630-104">เมื่อใช้ฟีเจอร์นี้ Azure AD จะกำหนดค่ากฎการซิงโครไนซ์โดยอัตโนมัติดังนี้</span><span class="sxs-lookup"><span data-stu-id="d9630-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="d9630-105">ใช้ msDS-ConsistencyGuid เป็นแอตทริบิวต์ sourceAnchor สำหรับวัตถุของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="d9630-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="d9630-106">ObjectGUID ถูกใช้สำหรับชนิดวัตถุอื่น</span><span class="sxs-lookup"><span data-stu-id="d9630-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="d9630-107">สำหรับวัตถุผู้ใช้โฆษณาภายในองค์กรที่มีแอตทริบิวต์ msDS-ConsistencyGuid ไม่ถูกเติมข้อมูล Azure AD Connect จะเขียนค่า objectGUID กลับไปยังแอตทริบิวต์ msDS-ConsistencyGuid ใน active Directory ภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="d9630-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="d9630-108">หลังจากที่มีการเติมแอตทริบิวต์ msDS-ConsistencyGuid แล้ว Azure AD Connect จะส่งออกวัตถุไปยัง AD Azure</span><span class="sxs-lookup"><span data-stu-id="d9630-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="d9630-109">**หมายเหตุ:** เมื่อวัตถุของโฆษณาภายในองค์กรถูกนำเข้าไปยัง Azure AD Connect (ซึ่งถูกนำเข้าลงในพื้นที่ตัวเชื่อมต่อของโฆษณาและคาดการณ์ไว้ใน Metaverse) คุณจะไม่สามารถเปลี่ยนแปลงค่า sourceAnchor ได้อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="d9630-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="d9630-110">เมื่อต้องการระบุค่า sourceAnchor สำหรับวัตถุโฆษณาในสถานที่ที่กำหนดให้กำหนดค่าแอตทริบิวต์ msDS ของ ConsistencyGuid ก่อนที่จะนำเข้าลงใน Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="d9630-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="d9630-111">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ SourceAnchor และ ConsistencyGuid ให้ดูดังต่อไปนี้: การ [เชื่อมต่อ AZURE AD: แนวคิดการออกแบบ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="d9630-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

