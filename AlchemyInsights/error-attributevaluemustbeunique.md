---
title: ข้อผิดพลาด AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709170"
---
# <a name="error-attributevaluemustbeunique"></a>ข้อผิดพลาด: AttributeValueMustBeUnique

สาเหตุทั่วไปของข้อผิดพลาด AttributeValueMustBeUnique คือวัตถุสองวัตถุที่มี SourceAnchor ที่แตกต่างกัน (immutableId) มีค่าเดียวกันสำหรับแอตทริบิวต์ ProxyAddresses และ/หรือ UserPrincipalName เมื่อต้องการแก้ไขข้อผิดพลาด AttributeValueMustBeUnique:
  
1. ระบุการ proxyAddresses ที่ซ้ำกัน userPrincipalName หรือค่าแอตทริบิวต์อื่นๆที่เป็นสาเหตุของข้อผิดพลาด นอกจากนี้ระบุวัตถุสองอย่าง (หรือมากกว่า) ที่เกี่ยวข้องกับข้อขัดแย้ง รายงานที่สร้างขึ้นโดย Azure AD Connect Health for sync สามารถช่วยให้คุณระบุวัตถุสองวัตถุได้
    
2. ระบุว่าวัตถุใดควรมีค่าที่ซ้ำกันและวัตถุใดที่ไม่ควรทำ
    
3. เอาค่าที่ซ้ำกันออกจากวัตถุที่ไม่ควรมีค่านั้น โปรดสังเกตว่าคุณควรทำการเปลี่ยนแปลงในไดเรกทอรีที่วัตถุนั้นมีที่มาจาก ในบางกรณีคุณอาจจำเป็นต้องลบวัตถุใดวัตถุหนึ่งในข้อขัดแย้ง
    
4. ถ้าคุณทำการเปลี่ยนแปลงในโฆษณาภายในองค์กรให้ Azure AD Connect การซิงค์การเปลี่ยนแปลงเพื่อให้ได้รับการแก้ไขข้อผิดพลาด
    

