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
# <a name="consistencyguid--sourceanchor-behavior"></a>ลักษณะการทำงานของ ConsistencyGuid/แหล่งที่ยึด

การเชื่อมต่อ AD Azure (รุ่น1.1.524.0 และหลังจาก) ในขณะนี้อำนวยความสะดวกในการใช้งานของ msDS ConsistencyGuid เป็นแอตทริบิวต์ sourceAnchor เมื่อใช้คุณลักษณะนี้การเชื่อมต่อ AD Azure กำหนดค่ากฎการซิงโครไนส์โดยอัตโนมัติเพื่อ:
  
- ใช้ msDS-ConsistencyGuid เป็นแอตทริบิวต์ sourceAnchor สำหรับวัตถุผู้ใช้ ObjectGUID จะใช้สำหรับชนิดออบเจ็กต์อื่น
    
- สำหรับวัตถุใดๆที่กำหนดไว้ในสถานที่ผู้ใช้โฆษณาแอตทริบิวต์ ConsistencyGuid ไม่ได้บรรจุ, การเชื่อมต่อ AD Azure เขียนค่า objectGUID ของมันกลับไปยังแอตทริบิวต์ msDS-ConsistencyGuid ในไดเรกทอรีที่ใช้งานอยู่ในสถาน หลังจากที่มีรวบรวมแอตทริบิวต์ ConsistencyGuid การเชื่อมต่อ AD Azure แล้วส่งออกวัตถุไปยังโฆษณา Azure
    
 **หมายเหตุ:** เมื่อมีการนำเข้าวัตถุโฆษณาในสถานที่ในการเชื่อมต่อ AD Azure (นั่นคือนำเข้าลงในพื้นที่ตัวเชื่อมต่อ AD และคาดการณ์ไว้ใน Metaverse) คุณจะไม่สามารถเปลี่ยนแปลงแหล่งที่มาของจุดยึดอีกต่อไป เมื่อต้องการระบุค่า sourceAnchor สำหรับวัตถุโฆษณาในสถานที่ที่กำหนดให้กำหนดค่าแอตทริบิวต์ ConsistencyGuid ก่อนที่จะนำเข้ามาในการเชื่อมต่อ AD Azure 
  
สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ SourceAnchor และ ConsistencyGuid อ้างอิงถึงต่อไปนี้:[แนวคิดการออกแบบโฆษณา Azure:](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

