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
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7b98b68fabff6c048f1bab6cf506355114d18658
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916543"
---
# <a name="error-attributevaluemustbeunique"></a>ข้อผิดพลาด: AttributeValueMustBeUnique

สาเหตุทั่ว ๆ ไปสำหรับข้อผิดพลาด AttributeValueMustBeUnique เป็นวัตถุสองวัตถุที่ มี SourceAnchor ที่แตกต่างกัน (immutableId) มีค่าเดียวกันสำหรับแอตทริบิวต์ ProxyAddresses และ/หรือ UserPrincipalName เมื่อต้องการแก้ไขข้อผิดพลาด AttributeValueMustBeUnique:
  
1. ระบุการ proxyAddresses ซ้ำ userPrincipalName หรือค่าแอททริบิวต์อื่น ๆ ที่เป็นสาเหตุของข้อผิดพลาด นอกจากนี้ยัง ระบุวัตถุที่สอง (หรือมากกว่า) ที่เกี่ยวข้องกับความขัดแย้ง รายงานสร้างขึ้น โดย Azure โฆษณาเชื่อมต่อความสมบูรณ์สำหรับการซิงค์สามารถช่วยคุณในการระบุออบเจ็กต์สอง
    
2. ระบุวัตถุใดควรดำเนินต่อเพื่อให้ค่าที่ซ้ำกันและวัตถุที่ไม่ควร
    
3. เอาค่าซ้ำกันออกจากวัตถุที่ไม่ควรมีค่านั้น หมายเหตุว่า คุณควรทำการเปลี่ยนแปลงในไดเรกทอรีที่วัตถุที่เป็นต้นทางจาก ในบางกรณี คุณอาจต้องการลบวัตถุหนึ่งเกิดความขัดแย้ง
    
4. ถ้าคุณทำการเปลี่ยนแปลงในสถานในโฆษณา ให้เชื่อมต่อ AD Azure ซิงค์การเปลี่ยนแปลงสำหรับข้อผิดพลาดจะได้รับการแก้ไข
    

