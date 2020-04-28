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
ms.openlocfilehash: d37fd903c91c8cd6ac6137e815cb253f7edb4494
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912694"
---
# <a name="restore-a-deleted-site"></a>คืนค่าไซต์ที่ถูกลบ

เมื่อผู้ดูแลระบบลบไซต์ SharePoint ไซต์นั้นจะถูกวางไว้ในถังรีไซเคิลของไซต์คอลเลกชัน ซึ่งถูกเก็บไว้เป็นเวลา 93 วันก่อนที่จะถูกลบอย่างถาวร เมื่อต้องการคืนค่าไซต์:
  
1. ในศูนย์การจัดการ SharePoint ใหม่ ให้คลิก**ถังรีไซเคิล**บน Ribbon 
    
2. เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากไซต์คอลเลกชันที่คุณต้องการคืนค่า
    
3. คลิก**คืนค่ารายการที่ถูกลบ**
    
เมื่อต้องการคืนค่าไซต์การสื่อสารที่ถูกลบ มิฉะนั้น คุณจําเป็นต้องใช้ Microsoft PowerShell เมื่อต้องการคืนค่าไซต์ที่เป็นสมาชิกของกลุ่ม Microsoft 365 คุณต้องคืนค่ากลุ่มในศูนย์การจัดการ Exchange กลุ่มสามารถเรียกคืนได้เป็นเวลา 30 วันหลังจากที่ลบ
  

