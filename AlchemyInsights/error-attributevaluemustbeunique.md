---
title: Error AttributeValuMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002144"
---
# <a name="error-attributevaluemustbeunique"></a>ข้อผิดพลาด: AttributeValusMustBeUnique

เหตุผลที่ใช้กันมากที่สุดของข้อผิดพลาด AttributeValusMustBeUnique คือวัตถุสองรายการที่มี SourceAnchor ที่ต่างกัน (immutableId) มีค่าเดียวกันนี้กับแอตทริบิวต์ ProxyAddresses และ/หรือ UserPrincipalName เมื่อต้องการแก้ไขข้อผิดพลาด AttributeValusMustBeUnique:
  
1. ระบุ proxyAddresses ที่ซ้นแล้ว userPrincipalName หรือค่าแอตทริบิวต์อื่นๆ ที่ทําให้เกิดข้อผิดพลาด นอกจากนี้ ให้ระบุว่าวัตถุสองรายการ (หรือมากกว่านั้น) รายการใดที่เกี่ยวข้องในข้อขัดแย้งนี้ รายงานที่สร้างขึ้นโดย Azure AD เชื่อมต่อ Health for sync สามารถช่วยคุณระบุวัตถุทั้งสองรายการได้
    
2. ระบุว่าวัตถุใดควรมีค่าที่คัดลอกไว้ต่อและวัตถุใดไม่ควรถูกคัดลอก
    
3. เอาค่าที่คัดลอกออกจากวัตถุที่ไม่ควรมีค่าดังกล่าว โปรดทราบว่าคุณควรเปลี่ยนแปลงในไดเรกทอรีที่มีวัตถุมาจาก ในบางกรณี คุณอาจต้องลบหนึ่งในวัตถุที่ขัดแย้งกัน
    
4. ถ้าคุณเปลี่ยนแปลงใน AD ภายในองค์กร ให้ปล่อยให้ Azure AD เชื่อมต่อซิงค์การเปลี่ยนแปลงเพื่อให้ข้อผิดพลาดได้รับการแก้ไข
    

