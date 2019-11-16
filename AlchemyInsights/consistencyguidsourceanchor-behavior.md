---
title: ลักษณะการทำงานของ ConsistencyGuid/แหล่งที่ยึด
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/15/2019
ms.locfileid: "36517014"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="61a6b-102">ลักษณะการทำงานของ ConsistencyGuid/แหล่งที่ยึด</span><span class="sxs-lookup"><span data-stu-id="61a6b-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="61a6b-103">การเชื่อมต่อ AD Azure (รุ่น1.1.524.0 และหลังจาก) ในขณะนี้อำนวยความสะดวกในการใช้งานของ msDS ConsistencyGuid เป็นแอตทริบิวต์ sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="61a6b-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="61a6b-104">เมื่อใช้คุณลักษณะนี้การเชื่อมต่อ AD Azure กำหนดค่ากฎการซิงโครไนส์โดยอัตโนมัติเพื่อ:</span><span class="sxs-lookup"><span data-stu-id="61a6b-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="61a6b-105">ใช้ msDS-ConsistencyGuid เป็นแอตทริบิวต์ sourceAnchor สำหรับวัตถุผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="61a6b-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="61a6b-106">ObjectGUID จะใช้สำหรับชนิดออบเจ็กต์อื่น</span><span class="sxs-lookup"><span data-stu-id="61a6b-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="61a6b-107">สำหรับวัตถุใดๆที่กำหนดไว้ในสถานที่ผู้ใช้โฆษณาแอตทริบิวต์ ConsistencyGuid ไม่ได้บรรจุ, การเชื่อมต่อ AD Azure เขียนค่า objectGUID ของมันกลับไปยังแอตทริบิวต์ msDS-ConsistencyGuid ในไดเรกทอรีที่ใช้งานอยู่ในสถาน</span><span class="sxs-lookup"><span data-stu-id="61a6b-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="61a6b-108">หลังจากที่มีรวบรวมแอตทริบิวต์ ConsistencyGuid การเชื่อมต่อ AD Azure แล้วส่งออกวัตถุไปยังโฆษณา Azure</span><span class="sxs-lookup"><span data-stu-id="61a6b-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="61a6b-109">**หมายเหตุ:** เมื่อมีการนำเข้าวัตถุโฆษณาในสถานที่ในการเชื่อมต่อ AD Azure (นั่นคือนำเข้าลงในพื้นที่ตัวเชื่อมต่อ AD และคาดการณ์ไว้ใน Metaverse) คุณจะไม่สามารถเปลี่ยนแปลงแหล่งที่มาของจุดยึดอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="61a6b-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="61a6b-110">เมื่อต้องการระบุค่า sourceAnchor สำหรับวัตถุโฆษณาในสถานที่ที่กำหนดให้กำหนดค่าแอตทริบิวต์ ConsistencyGuid ก่อนที่จะนำเข้ามาในการเชื่อมต่อ AD Azure</span><span class="sxs-lookup"><span data-stu-id="61a6b-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="61a6b-111">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ SourceAnchor และ ConsistencyGuid อ้างอิงถึงต่อไปนี้:[แนวคิดการออกแบบโฆษณา Azure:](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="61a6b-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

