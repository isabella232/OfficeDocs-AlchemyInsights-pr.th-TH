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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044360"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ลักษณะการสอดคล้องGuid / sourceAnchor

ขณะนี้ Azure AD เชื่อมต่อ (เวอร์ชัน 1.1.524.0 และหลังจากนั้น) จะอ่วยความสะดวกในการใช้แอตทริบิวต์ msDS-ConsistencyGuid เป็นแอตทริบิวต์ SourceAnchor เมื่อใช้ฟีเจอร์นี้ Azure AD จะเชื่อมต่อกฎการซิงโครไนซ์โดยอัตโนมัติเพื่อ:
  
- ใช้ msDS-ConsistencyGuid เป็นแอตทริบิวต์ SourceAnchor ของวัตถุผู้ใช้ ObjectGUID จะถูกใช้กับวัตถุชนิดอื่นๆ
    
- For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD เชื่อมต่อ writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. หลังจากสร้างแอตทริบิวต์ msDS-ConsistencyGuid แล้ว เชื่อมต่อ Azure AD จะส่งออกวัตถุไปยัง Azure AD
    
 **หมายเหตุ:** เมื่อนําเข้าวัตถุ AD ภายในองค์กรลงใน Azure AD เชื่อมต่อ (ซึ่งถูกนําเข้าลงในพื้นที่ตัวเชื่อมต่อ AD และที่ฉายลงใน Metaverse) คุณจะไม่สามารถเปลี่ยนค่า SourceAnchor ของวัตถุได้อีกต่อไป เมื่อต้องการระบุค่า SourceAnchor ของวัตถุ AD ภายในองค์กรที่กําหนด ให้กําหนดค่าแอตทริบิวต์ msDS-ConsistencyGuid ของวัตถุก่อนที่จะถูกนําเข้าลงในเชื่อมต่อ Azure AD 
  
For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD เชื่อมต่อ: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

