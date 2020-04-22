---
title: ข้อผิดพลาดของแอตทริบิวต์ค่าต้องไม่ซ้ํา
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703193"
---
# <a name="error-attributevaluemustbeunique"></a>ข้อผิดพลาด: ค่าแอตทริบิวต์ต้องไม่ซ้ํากัน

เหตุผลทั่วไปมากที่สุดสําหรับข้อผิดพลาด AttributeValueMustBeUnique คือวัตถุสองออบเจ็กต์กับ SourceAnchor (immutableId) แตกต่างกันมีค่าเดียวกันสําหรับการProxyAddressesและ/หรือแอตทริบิวต์ UserPrincipalName เมื่อต้องการแก้ไขข้อผิดพลาด AttributeValueMustBeUnique:
  
1. ระบุ proxyAddresses, userPrincipalName หรือค่าแอตทริบิวต์อื่น ๆ ที่ก่อให้เกิดข้อผิดพลาด นอกจากนี้ระบุวัตถุ (หรือมากกว่า) สองที่เกี่ยวข้องกับความขัดแย้ง รายงานที่สร้างขึ้น โดย Azure AD Connect Health สําหรับการซิงค์ สามารถช่วยให้คุณระบุวัตถุสองตัวได้
    
2. ระบุว่าวัตถุใดที่ควรยังคงมีค่าที่ซ้ํากันและวัตถุใดที่ไม่ควร
    
3. เอาค่าที่ซ้ํากันจากวัตถุที่ไม่ควรมีค่านั้น โปรดสังเกตว่า คุณควรทําการเปลี่ยนแปลงในไดเรกทอรีที่วัตถุต้นทางจาก ในบางกรณี คุณอาจต้องลบวัตถุใดวัตถุหนึ่งที่มีข้อขัดแย้ง
    
4. ถ้าคุณทําการเปลี่ยนแปลงในสถานที่ในการโฆษณา ให้ Azure AD Connect ซิงค์การเปลี่ยนแปลงสําหรับข้อผิดพลาดเพื่อได้รับการแก้ไข
    

