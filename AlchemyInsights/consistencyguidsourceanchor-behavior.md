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
# <a name="consistencyguid--sourceanchor-behavior"></a>ลักษณะการสอดคล้องGuid / sourceAnchor

Azure AD Connect (เวอร์ชัน 1.1.524.0 และหลังจากนั้น) ช่วยให้การใช้ msDS-ConsistencyGuid เป็นแอตทริบิวต์ SourceAnchor ง่ายขึ้น เมื่อใช้ฟีเจอร์นี้ Azure AD Connect จะกําหนดค่ากฎการซิงโครไนซ์ให้โดยอัตโนมัติ:
  
- ใช้ msDS-ConsistencyGuid เป็นแอตทริบิวต์ SourceAnchor ของวัตถุผู้ใช้ ObjectGUID จะถูกใช้กับวัตถุชนิดอื่นๆ
    
- For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. หลังจากสร้างแอตทริบิวต์ msDS-ConsistencyGuid แล้ว Azure AD Connect จะส่งออกวัตถุไปยัง Azure AD
    
 **หมายเหตุ:** เมื่อนําเข้าวัตถุ AD ภายในองค์กรลงใน Azure AD Connect (ซึ่งนําเข้าลงในพื้นที่ตัวเชื่อมต่อ AD และที่ฉายลงใน Metaverse) คุณจะไม่สามารถเปลี่ยนค่า SourceAnchor ของวัตถุได้อีกต่อไป เมื่อต้องการระบุค่า SourceAnchor ของวัตถุ AD ภายในองค์กรที่กําหนด ให้กําหนดค่าแอตทริบิวต์ msDS-ConsistencyGuid ของวัตถุก่อนที่จะถูกนําเข้าลงใน Azure AD Connect 
  
For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

