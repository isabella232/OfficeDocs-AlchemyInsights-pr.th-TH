---
title: คืนค่าไซต์ที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 8f9a5f78c1a0eae2632fbf7c5132e520847feef415f7b6887d5d7796af720304
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958856"
---
# <a name="restore-a-deleted-site"></a>คืนค่าไซต์ที่ถูกลบ

เมื่อผู้ดูแลระบบลบไซต์ SharePoint ไซต์ของคุณ ไซต์นั้นจะถูกวางในถังรีไซเคิลของไซต์คอลเลกชันที่จะถูกเก็บไว้เป็นเวลา 93 วันก่อนที่ไซต์นั้นจะถูกลบอย่างถาวร เมื่อต้องการคืนค่าไซต์ ให้ต่อไปนี้
  
1. ในศูนย์SharePointการจัดการ ให้คลิก **ถัง** รีไซเคิล บน Ribbon 
    
2. เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากไซต์คอลเลกชันที่คุณต้องการคืนค่า
    
3. คลิก **คืนค่ารายการ** ที่ถูกลบ
    
เมื่อต้องการคืนค่าไซต์การติดต่อสื่อสารที่ถูกลบ คุณสามารถใช้ศูนย์SharePointผู้ดูแลระบบใหม่ได้ มิฉะนั้น คุณต้องใช้ Microsoft PowerShell เมื่อต้องการคืนค่าไซต์ที่เป็นของกลุ่มMicrosoft 365 คุณจึงต้องคืนค่ากลุ่มในศูนย์Exchangeการจัดการ คุณสามารถคืนค่ากลุ่มได้ภายใน 30 วันหลังจากที่ถูกลบ
  

