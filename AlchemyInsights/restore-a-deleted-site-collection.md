---
title: คืนค่าไซต์ถูกลบไปแล้ว
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 0cf10a3a0effc1774d8a07c5d0be96384362c175
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747797"
---
# <a name="restore-a-deleted-site"></a>คืนค่าไซต์ถูกลบไปแล้ว

เมื่อผู้ดูแลระบบการลบไซต์ ถูกวางไว้ในไซต์คอลเลกชันถังรีไซเคิล ซึ่งจะถูกเก็บอยู่ 93 วันก่อนที่จะถูกลบออกอย่างถาวร เมื่อต้องการคืนค่าไซต์:
  
1. ในศูนย์การดูแล SharePoint ใหม่คลิก **'ถังรีไซเคิล'** ใน ribbon 
    
2. เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากไซต์คอลเลกชันที่คุณต้องการคืนค่า
    
3. คลิก**เรียกคืนรายการที่ถูกลบไปแล้ว**
    
เมื่อต้องการคืนค่าไซต์การสื่อสารที่ถูกลบไปแล้ว คุณสามารถใช้ศูนย์กลางการดูแล SharePoint ใหม่ มิฉะนั้น คุณจำเป็นต้องใช้ Microsoft PowerShell เมื่อต้องการคืนค่าไซต์ที่เป็นสมาชิกของกลุ่มมี Office 365 คุณต้องคืนค่ากลุ่มในศูนย์ดูแลการแลกเปลี่ยน กลุ่มสามารถคืนค่าได้เท่ากับ 30 วันหลังจากที่พวกเขากำลังถูกลบ
  

