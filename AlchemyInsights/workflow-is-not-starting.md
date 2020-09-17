---
title: เวิร์กโฟลว์ไม่เริ่มทำงาน
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794786"
---
# <a name="workflow-is-not-starting"></a>เวิร์กโฟลว์ไม่เริ่มทำงาน

- เวิร์กโฟลว์ SharePoint ๒๐๑๐และ SharePoint ๒๐๑๓จะไม่เริ่มทำงาน

    - ถ้าเวิร์กโฟลว์ของคุณไม่ได้เริ่มทำงานอาจมีปัญหาในการบริการชั่วคราวที่ผู้ใช้อาจพบความล่าช้าเป็นระยะๆด้วยความคืบหน้าของเวิร์กโฟลว์ ตรวจสอบ [แดชบอร์ดความสมบูรณ์ของบริการ](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่

    - ถ้าคุณได้รับการส่งผ่านมากกว่า24ชั่วโมงหลังจากที่คุณเห็นปัญหานี้ครั้งแรกโปรดเข้าสู่ระบบตั๋วสนับสนุน ในหลายกรณีเรากำลังทำงานกับโซลูชันอยู่แล้ว โปรดแจ้งให้เราทราบอย่างน้อย24ชั่วโมงเพื่อให้โซลูชันเสร็จสมบูรณ์

- เวิร์กโฟลว์ SharePoint ๒๐๑๐ล่าช้าเมื่อเริ่มต้น

    - เหตุการณ์นี้จะเกิดขึ้นถ้าเวิร์กโฟลว์ถูกทริกเกอร์ในชุดขนาดใหญ่ (ตัวอย่างเช่นเมื่อมีการเพิ่มรายการหลายรายการในครั้งเดียว)

    - เวิร์กโฟลว์ไม่ได้รับการออกแบบมาให้ทำงานแบบเรียลไทม์ดังนั้นการหน่วงเวลาคือการทำงานโดยการออกแบบ

   -  ถ้าเวิร์กโฟลว์เป็นภาษาที่ซับซ้อน Extensible Object Markup Language (XMOL) การคอมไพล์สามารถทำงานได้ช้า ตรวจสอบบทความ[นี้](https://support.microsoft.com//kb/3043697)

    - คุณควรทำให้เวิร์กโฟลว์ทำงานได้ง่ายขึ้นหรือออกแบบใหม่โดยใช้ชนิดของแพลตฟอร์มสำหรับเวิร์กโฟลว์ของ Microsoft SharePoint ๒๐๑๓

    - ถ้าประวัติเวิร์กโฟลว์ของคุณมีขนาดใหญ่ขึ้นคุณอาจต้องการล้างข้อมูลรายการหรือสร้างรายการประวัติใหม่

        ข้อมูลเพิ่มเติม: การ [ล้างประวัติของเวิร์กโฟลว์](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
ต้องการลองใช้ Microsoft Flow ใน SharePoint Online หรือไม่
- [สร้างขั้นตอน](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint และการไหล](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


