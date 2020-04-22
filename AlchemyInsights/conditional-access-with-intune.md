---
title: การเข้าถึงแบบมีเงื่อนไขด้วย Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706040"
---
# <a name="conditional-access-with-intune"></a>การเข้าถึงแบบมีเงื่อนไขด้วย Intune

การใช้**การเข้าถึงแบบมีเงื่อนไข**กับ Intune ต้องใช้ 3 ขั้นตอน: 
  
- สร้าง**นโยบายการเข้าถึงแบบมีเงื่อนไข**ที่กําหนดทรัพยากรใดที่จะถูกป้องกัน และเงื่อนไขที่จําเป็นต้องได้รับเพื่อเข้าถึงทรัพยากรเหล่านั้น ตัวอย่างเช่น อุปกรณ์ต้องเป็นไปตามข้อกําหนดก่อนเข้าถึงอีเมลของบริษัท 
    
- สร้าง**นโยบายการปฏิบัติตามกฎระเบียบ**เพื่อกําหนดการตั้งค่าที่ต้องเป็นไปตามก่อนที่อุปกรณ์จะถือว่าสอดคล้อง ตัวอย่างเช่น อุปกรณ์ต้องมีหมุดอย่างน้อย 6 หลักก่อนที่จะถือว่าเป็นไปตามข้อกําหนด 
    
- การทําให้แน่ใจว่า**นโยบายการปฏิบัติตามกฎระเบียบ**และ**นโยบายการเข้าถึงแบบมีเงื่อนไข**จะกําหนดเป้าหมายไปยังกลุ่มผู้ใช้ที่ต้องการ ซึ่งอาจต้องการสร้างกลุ่มเฉพาะของผู้ใช้ในไดเรกทอรีที่ใช้งานอยู่ของ Azure 
    
อ่านเพิ่มเติม:
  
- [แนวทางปฏิบัติที่ดีที่สุดของการเข้าถึงแบบมีเงื่อนไข](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [การเริ่มต้นใช้งานการเข้าถึงแบบมีเงื่อนไข](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

