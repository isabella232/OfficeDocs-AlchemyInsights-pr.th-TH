---
title: ไม่สามารถเข้าถึงไซต์นี้ - ข้อผิดพลาดเมื่อพยายามเข้าถึงSharePointจากเบราว์เซอร์หรือTeams
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
ms.openlocfilehash: 5f8861e85df21082329273237679e26a1b31ce694e11ad6407d4690d7caf2fc9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946670"
---
# <a name="this-site-cant-be-reached-error-when-trying-to-access-sharepoint-site-from-browser-or-teams"></a>ข้อผิดพลาด "ไม่สามารถเข้าถึงไซต์นี้" เมื่อพยายามเข้าถึงไซต์SharePointจากเบราว์เซอร์หรือTeams

ผู้ใช้อาจได้รับข้อผิดพลาด "ไม่สามารถเข้าถึงไซต์นี้" เมื่อพยายามเข้าถึงSharePointจากเบราว์เซอร์หรือTeams 

เมื่อต้องการแก้ไขปัญหานี้: 

1. ตรวจสอบว่าโฮมเพจอยู่ในถังรีไซเคิลหรือถังรีไซเคิลขั้นที่สองและคืนค่าหน้า

**ตัวอย่าง URL โดยตรงไปยังถังรีไซเคิล**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx

1. ถ้าโฮมเพจถูกเอาออกจากถังรีไซเคิลอย่างถาวร ให้สร้างหน้าไซต์ใหม่จากไลบรารี หน้าไซต์ แล้วสร้างโฮมเพจ 

**ตัวอย่าง URL โดยตรง**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx