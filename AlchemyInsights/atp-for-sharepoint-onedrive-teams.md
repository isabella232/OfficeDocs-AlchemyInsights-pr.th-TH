---
title: ATP สําหรับ SharePoint, วันไดรฟ์ และทีมไมโครซอฟท์
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508431"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP สําหรับ SharePoint, วันไดรฟ์ และทีมไมโครซอฟท์

ทําตามขั้นตอนเหล่านี้เพื่อเปิดใช้งานการป้องกันภัยคุกคามขั้นสูง:

1. ไปที่ [https://protection.office.com](https://protection.office.com) และลงชื่อเข้าใช้ด้วยบัญชีผู้ดูแลระบบส่วนกลางหรือผู้ดูแลความปลอดภัย

2. ในบานหน้าต่างการนําทางด้านซ้ายภายใต้**การจัดการภัยคุกคาม**ให้เลือก**Policy** \> **สิ่งที่แนบมาที่ปลอดภัย**ของนโยบาย

3. เลือก**เปิด ATP สําหรับ SharePoint, OneDrive และ ทีม Microsoft**

4. [สร้างนโยบายการแจ้งเตือนกิจกรรม](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts)เพื่อรับการแจ้งเตือนเมื่อเราตรวจพบไฟล์ที่เป็นอันตราย

สําหรับคําแนะนําทั้งหมด โปรดดูที่[หัวข้อนี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)

**หมายเหตุ**: โดยการออกแบบ ATP ไม่สแกนทุกไฟล์เดียวใน SharePoint แบบออนไลน์, OneDrive สําหรับธุรกิจ หรือทีมของ Microsoft ไฟล์จะถูกสแกนแบบอะซิงโครนัสโดยกระบวนการที่ใช้กิจกรรมร่วมกัน กิจกรรมของผู้เยี่ยมชม และสัญญาณภัยคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย สําหรับข้อมูลเพิ่มเติม ให้ดูที่[หัวข้อนี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
