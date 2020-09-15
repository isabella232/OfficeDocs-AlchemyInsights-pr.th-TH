---
title: การคืนค่าไซต์ที่ถูกลบ
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
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692062"
---
# <a name="restore-a-deleted-site"></a>การคืนค่าไซต์ที่ถูกลบ

เมื่อผู้ดูแลระบบลบไซต์ SharePoint แล้วไฟล์นั้นจะถูกวางไว้ในถังรีไซเคิลของไซต์คอลเลกชันซึ่งจะถูกเก็บไว้สำหรับ๙๓วันก่อนที่จะถูกลบออกอย่างถาวร เมื่อต้องการคืนค่าไซต์:
  
1. ในศูนย์การจัดการ SharePoint ใหม่ให้คลิกถัง **รีไซเคิล** บน ribbon 
    
2. เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากไซต์คอลเลกชันที่คุณต้องการคืนค่า
    
3. คลิก**คืนค่ารายการที่ถูกลบ**
    
เมื่อต้องการคืนค่าไซต์การติดต่อสื่อสารที่ถูกลบคุณสามารถใช้ศูนย์การจัดการ SharePoint ใหม่ได้ มิฉะนั้นคุณจำเป็นต้องใช้ Microsoft PowerShell เมื่อต้องการคืนค่าไซต์ที่เป็นสมาชิกของกลุ่ม Microsoft ๓๖๕คุณจำเป็นต้องคืนค่ากลุ่มในศูนย์การจัดการ Exchange กลุ่มสามารถคืนค่าเป็นเวลา30วันหลังจากที่ถูกลบไปแล้ว
  

