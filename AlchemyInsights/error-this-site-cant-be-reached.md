---
title: ไม่สามารถเข้าถึงไซต์นี้ - ข้อผิดพลาดเมื่อพยายามเข้าถึงไซต์ SharePoint จากเบราว์เซอร์หรือ Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005378"
- "9266"
ms.openlocfilehash: 451544fb85522e0eececc9274825805699685ee9
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747036"
---
# <a name="this-site-cant-be-reached-error-when-trying-to-access-sharepoint-site-from-browser-or-teams"></a>ข้อผิดพลาด "ไม่สามารถเข้าถึงไซต์นี้" เมื่อพยายามเข้าถึงไซต์ SharePoint จากเบราว์เซอร์หรือ Teams

ผู้ใช้อาจได้รับข้อผิดพลาด "ไม่สามารถเข้าถึงไซต์นี้" เมื่อพยายามเข้าถึงไซต์ SharePoint จากเบราว์เซอร์หรือ Teams 

เมื่อต้องการแก้ไขปัญหานี้: 

1. ตรวจสอบว่าโฮมเพจอยู่ในถังรีไซเคิลหรือถังรีไซเคิลขั้นที่สองและคืนค่าหน้า

**ตัวอย่าง URL โดยตรงไปยังถังรีไซเคิล**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx

1. ถ้าโฮมเพจถูกเอาออกจากถังรีไซเคิลอย่างถาวร ให้สร้างหน้าไซต์ใหม่จากไลบรารีหน้าไซต์แล้วสร้างโฮมเพจ 

**ตัวอย่าง URL โดยตรง**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx