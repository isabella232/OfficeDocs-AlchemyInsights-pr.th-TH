---
title: การเข้าถึงแบบมีเงื่อนไขกับ Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36505013"
---
# <a name="conditional-access-with-intune"></a>การเข้าถึงแบบมีเงื่อนไขกับ Intune

การใช้การ**เข้าถึง**แบบมีเงื่อนไขกับ Intune ต้องการขั้นตอน 3: 
  
- สร้าง**นโยบายการเข้าถึง**แบบมีเงื่อนไขที่กำหนดว่าทรัพยากรใดได้รับการป้องกันและจะต้องพบกับเงื่อนไขใดบ้างในการเข้าถึงทรัพยากรเหล่านั้น ตัวอย่างเช่นอุปกรณ์ต้องสอดคล้องกันก่อนที่จะเข้าถึงเมลของบริษัท 
    
- สร้าง**นโยบายการปฏิบัติตามกฎระเบียบ**เพื่อกำหนดการตั้งค่าที่ต้องได้รับก่อนที่อุปกรณ์จะถือว่าเป็นไปตามมาตรฐาน ตัวอย่างเช่นอุปกรณ์ต้องมี pin อย่างน้อย6หลักก่อนที่จะถือว่าเป็นไปตามมาตรฐาน 
    
- การสร้างความมั่นใจใน**นโยบายการปฏิบัติตามกฎระเบียบ**และ**นโยบายการเข้าถึง**แบบมีเงื่อนไขจะถูกกำหนดเป้าหมายไปยังกลุ่มผู้ใช้ที่ต้องการ ซึ่งอาจจำเป็นต้องสร้างกลุ่มผู้ใช้เฉพาะในไดเรกทอรีที่ใช้งานอยู่ของ Azure 
    
อ่านเพิ่มเติม:
  
- [แนวทางที่พึงปฏิบัติ](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [การเริ่มต้นใช้งานการเข้าถึงแบบมีเงื่อนไข](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

