---
title: ข้อผิดพลาด AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/15/2019
ms.locfileid: "36527074"
---
# <a name="error-attributevaluemustbeunique"></a>ข้อผิดพลาด: AttributeValueMustBeUnique

สาเหตุที่พบบ่อยที่สุดสำหรับข้อผิดพลาด AttributeValueMustBeUnique คือวัตถุสองอย่างที่มี SourceAnchor ที่แตกต่างกัน (immutableId) มีค่าเดียวกันสำหรับแอตทริบิวต์ ProxyAddresses และ/หรือ UserPrincipalName การแก้ไขข้อผิดพลาด AttributeValueMustBeUnique:
  
1. ระบุ proxyAddresses ที่ซ้ำกัน userPrincipalName หรือค่าแอตทริบิวต์อื่นๆที่เป็นสาเหตุของข้อผิดพลาด นอกจากนี้ยังระบุว่าวัตถุสอง (หรือมากกว่า) ที่มีส่วนเกี่ยวข้องในข้อขัดแย้ง รายงานที่สร้างโดย Azure AD Connect Health สำหรับการซิงค์สามารถช่วยคุณระบุวัตถุทั้งสอง
    
2. ระบุอ็อบเจ็กต์ที่ควรดำเนินการต่อเพื่อให้มีค่าที่ซ้ำกันและวัตถุที่ไม่ควร
    
3. เอาค่าที่ซ้ำกันออกจากวัตถุที่ไม่ควรมีค่านั้น หมายเหตุว่าคุณควรทำการเปลี่ยนแปลงในไดเรกทอรีที่วัตถุนั้นมาจาก ในบางกรณีคุณอาจต้องลบหนึ่งในวัตถุที่มีความขัดแย้ง
    
4. ถ้าคุณทำการเปลี่ยนแปลงในในสถานโฆษณาให้ Azure AD Connect ซิงค์การเปลี่ยนแปลงสำหรับข้อผิดพลาดที่จะได้รับการแก้ไข
    

