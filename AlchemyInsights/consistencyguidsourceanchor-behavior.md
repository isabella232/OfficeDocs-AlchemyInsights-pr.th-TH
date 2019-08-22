---
title: ConsistencyGuid / sourceAnchor ลักษณะการทำงาน
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517014"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="f3044-102">ConsistencyGuid / sourceAnchor ลักษณะการทำงาน</span><span class="sxs-lookup"><span data-stu-id="f3044-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="f3044-103">การเชื่อมต่อ AD azure (รุ่น 1.1.524.0 และหลัง) เอื้อการใช้เอกสาร msDS ConsistencyGuid เป็นแอตทริบิวต์ sourceAnchor ในขณะนี้</span><span class="sxs-lookup"><span data-stu-id="f3044-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="f3044-104">เมื่อต้องการใช้คุณลักษณะนี้ การเชื่อมต่อ AD Azure โดยอัตโนมัติคุณสามารถกำหนดค่ากฎการซิงโครไนส์กับ:</span><span class="sxs-lookup"><span data-stu-id="f3044-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="f3044-105">ใช้เอกสาร msDS ConsistencyGuid เป็นแอตทริบิวต์ sourceAnchor สำหรับวัตถุที่ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="f3044-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="f3044-106">ObjectGUID ถูกใช้สำหรับวัตถุชนิดอื่น</span><span class="sxs-lookup"><span data-stu-id="f3044-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="f3044-107">เนื่องจากสาเหตุใดที่กำหนดให้กับสถานผู้ใช้ AD วัตถุซึ่งมีแอตทริบิวต์ ConsistencyGuid เอกสาร msDS ไม่เขียนเชื่อมต่อ AD Azure มีการเติมข้อมูลค่า objectGUID กลับไปยังแอตทริบิวต์ ConsistencyGuid เอกสาร msDS ในไดเรกทอรีที่ใช้งานอยู่ในสถานนั้น</span><span class="sxs-lookup"><span data-stu-id="f3044-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="f3044-108">หลังจากที่มีแอตทริบิวต์ ConsistencyGuid เอกสาร msDS ข้อมูล เชื่อมต่อ AD Azure ส่งออกวัตถุไปยังโฆษณา Azure แล้ว</span><span class="sxs-lookup"><span data-stu-id="f3044-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="f3044-109">**หมายเหตุ:** หนึ่งครั้งผิดในสถานโฆษณาวัตถุถูกนำเข้ามายังเชื่อมต่อ AD Azure (ที่อยู่ นำเข้ามายังพื้นที่ตัวเชื่อมต่อ AD และที่คาดการณ์ไว้ใน Metaverse) คุณไม่สามารถเปลี่ยนแปลงค่าของ sourceAnchor อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="f3044-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="f3044-110">เมื่อต้องการระบุค่า sourceAnchor สำหรับการรับในสถานโฆษณาวัตถุ การกำหนดค่าของแอตทริบิวต์ ConsistencyGuid เอกสาร msDS ก่อนมีการนำเข้าลงในการเชื่อมต่อ AD Azure</span><span class="sxs-lookup"><span data-stu-id="f3044-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="f3044-111">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ SourceAnchor และ ConsistencyGuid อ้างอิงต่อไปนี้:[เชื่อมต่อ AD Azure: แนวคิดการออกแบบ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="f3044-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

