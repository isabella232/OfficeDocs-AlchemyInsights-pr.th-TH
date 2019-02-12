---
title: คืนค่าคอลเลกชันของไซต์ที่ถูกลบไปแล้ว
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 22fb513771abc1a604a347204bac268771cb9e37
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29940015"
---
# <a name="restore-a-deleted-site-collection"></a>คืนค่าคอลเลกชันของไซต์ที่ถูกลบไปแล้ว

เมื่อ admin การลบคอลเลกชันไซต์คลาสสิค ถูกวางไว้ในไซต์คอลเลกชันถังรีไซเคิล ซึ่งจะถูกเก็บอยู่ 93 วันก่อนที่จะถูกลบออกอย่างถาวร เมื่อต้องการคืนค่าไซต์คอลเลกชัน:
  
1. ในศูนย์ดูแลแบบคลาสสิกของ SharePoint คลิก **'ถังรีไซเคิล'** ใน ribbon 
    
2. เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากไซต์คอลเลกชันที่คุณต้องการคืนค่า
    
3. คลิก**เรียกคืนรายการที่ถูกลบไปแล้ว**
    
เมื่อต้องการคืนค่าไซต์การสื่อสารที่ถูกลบไปแล้ว คุณสามารถใช้ตัวอย่างศูนย์ดูแล SharePoint ใหม่ มิฉะนั้น คุณจำเป็นต้องใช้ PowerShell เมื่อต้องการคืนค่าไซต์ที่เป็นสมาชิกของกลุ่มมี Office 365 คุณต้องคืนค่ากลุ่มในศูนย์ดูแลการแลกเปลี่ยน กลุ่มสามารถคืนค่าได้เท่ากับ 30 วันหลังจากที่พวกเขากำลังถูกลบ
  

