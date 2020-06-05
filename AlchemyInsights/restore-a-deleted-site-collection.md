---
title: คืนค่าไซต์ที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 7c2ae754c86a3502092b622c55d18f3f4006bf8b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582254"
---
# <a name="restore-a-deleted-site"></a>คืนค่าไซต์ที่ถูกลบ

เมื่อผู้ดูแลลบไซต์ SharePoint ไซต์จะถูกวางไว้ในถังรีไซเคิลของไซต์คอลเลกชัน ซึ่งจะถูกเก็บไว้เป็นเวลา 93 วันก่อนที่ไซต์จะถูกลบอย่างถาวร เมื่อต้องการคืนค่าไซต์:
  
1. ในศูนย์การจัดการ SharePoint ใหม่ ให้คลิก**ถังรีไซเคิล**บน Ribbon 
    
2. เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากไซต์คอลเลกชันที่คุณต้องการคืนค่า
    
3. คลิก**คืนค่ารายการที่ถูกลบ**
    
เมื่อต้องการคืนค่าไซต์การสื่อสารที่ถูกลบ มิฉะนั้น คุณต้องใช้ Microsoft PowerShell เมื่อต้องการคืนค่าไซต์ที่เป็นสมาชิกของกลุ่ม Microsoft 365 คุณจําเป็นต้องคืนค่ากลุ่มในศูนย์การจัดการ Exchange กลุ่มสามารถเรียกคืนได้เป็นเวลา 30 วันหลังจากที่ลบกลุ่ม
  

