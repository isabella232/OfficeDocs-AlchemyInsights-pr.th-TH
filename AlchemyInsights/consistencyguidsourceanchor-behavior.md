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
# <a name="consistencyguid--sourceanchor-behavior"></a>ลักษณะการทำงาน ConsistencyGuid/sourceAnchor

Azure AD Connect (เวอร์ชัน1.1.524.0 และหลังจากนี้) จะอำนวยความสะดวกในการใช้งานของ msDS-ConsistencyGuid เป็นแอตทริบิวต์ sourceAnchor เมื่อใช้ฟีเจอร์นี้ Azure AD จะกำหนดค่ากฎการซิงโครไนซ์โดยอัตโนมัติดังนี้
  
- ใช้ msDS-ConsistencyGuid เป็นแอตทริบิวต์ sourceAnchor สำหรับวัตถุของผู้ใช้ ObjectGUID ถูกใช้สำหรับชนิดวัตถุอื่น
    
- สำหรับวัตถุผู้ใช้โฆษณาภายในองค์กรที่มีแอตทริบิวต์ msDS-ConsistencyGuid ไม่ถูกเติมข้อมูล Azure AD Connect จะเขียนค่า objectGUID กลับไปยังแอตทริบิวต์ msDS-ConsistencyGuid ใน active Directory ภายในองค์กร หลังจากที่มีการเติมแอตทริบิวต์ msDS-ConsistencyGuid แล้ว Azure AD Connect จะส่งออกวัตถุไปยัง AD Azure
    
 **หมายเหตุ:** เมื่อวัตถุของโฆษณาภายในองค์กรถูกนำเข้าไปยัง Azure AD Connect (ซึ่งถูกนำเข้าลงในพื้นที่ตัวเชื่อมต่อของโฆษณาและคาดการณ์ไว้ใน Metaverse) คุณจะไม่สามารถเปลี่ยนแปลงค่า sourceAnchor ได้อีกต่อไป เมื่อต้องการระบุค่า sourceAnchor สำหรับวัตถุโฆษณาในสถานที่ที่กำหนดให้กำหนดค่าแอตทริบิวต์ msDS ของ ConsistencyGuid ก่อนที่จะนำเข้าลงใน Azure AD Connect 
  
สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ SourceAnchor และ ConsistencyGuid ให้ดูดังต่อไปนี้: การ [เชื่อมต่อ AZURE AD: แนวคิดการออกแบบ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

