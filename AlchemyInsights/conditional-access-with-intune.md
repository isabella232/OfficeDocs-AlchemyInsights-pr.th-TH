---
title: การเข้าถึงแบบมีเงื่อนไขกับ Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 3b50bc96a879017b62e42e1849f72e68408a0d9d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662346"
---
# <a name="conditional-access-with-intune"></a>การเข้าถึงแบบมีเงื่อนไขกับ Intune

ใช้**การเข้าถึงแบบมีเงื่อนไข**กับ Intune ต้องมีขั้นตอนที่ 3: 
  
- สร้าง**นโยบายการเข้าถึงตามเงื่อนไข**ที่กำหนดทรัพยากรจะมีการป้องกัน และเงื่อนไขต้องมีสิ่งใดจะสามารถตอบสนองการเข้าถึงทรัพยากรดังกล่าว ตัวอย่างเช่น อุปกรณ์ต้องเข้ากันได้ก่อนที่จะเข้าถึงอีเมลขององค์กร 
    
- สร้าง**นโยบายการปฏิบัติตามกฎระเบียบ**เพื่อกำหนดการตั้งค่าที่เป็นเงื่อนไขก่อนที่อุปกรณ์จะถือว่าเป็นไปตามกฎ ตัวอย่างเช่น อุปกรณ์ต้องมี pin ของตัวเลขอย่างน้อย 6 หลักก่อนที่จะถือว่าเป็นไปตามกฎ 
    
- แน่ใจว่า ทั้ง**นโยบายการปฏิบัติตามกฎระเบียบ**และ**นโยบายการเข้าถึงแบบมีเงื่อนไข**จะมุ่งเป้าไปยังกลุ่มที่ต้องการของผู้ใช้ ซึ่งอาจจำเป็นต้องสร้างกลุ่มเฉพาะของผู้ใช้ในไดเรกทอรีที่ใช้งานอยู่ของ Azure 
    
อ่านเพิ่มเติม:
  
- [วิธีปฏิบัติที่ดีที่สุดเข้าแบบมีเงื่อนไข](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [เริ่มต้น ด้วยการเข้าถึงแบบมีเงื่อนไข](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

