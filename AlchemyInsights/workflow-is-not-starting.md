---
title: เวิร์กโฟลว์ไม่ได้เริ่มต้น
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403762"
---
# <a name="workflow-is-not-starting"></a>เวิร์กโฟลว์ไม่ได้เริ่มต้น

- เวิร์กโฟลว์ SharePoint 2010 และ SharePoint 2013 ไม่เริ่มขึ้น

    - ถ้าเวิร์กโฟลว์ของคุณไม่เริ่มขึ้น อาจมีปัญหาการบริการชั่วคราวที่ผู้ใช้อาจพบความล่าช้าในความคืบหน้าของเวิร์กโฟลว์เป็นระยะๆ ตรวจสอบ [แดชบอร์ดสถาน](https://admin.microsoft.com/AdminPortal/Home/servicehealth) ภาพบริการเพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่

    - หากเวลาผ่านไปมากกว่า 24 ชั่วโมงหลังจากที่คุณเห็นปัญหานี้เป็นครั้งแรก โปรดบันทึกตั๋วการสนับสนุน ในหลายกรณี เราหาวิธีแก้ไขแล้ว โปรดให้เวลาเราอย่างน้อย 24 ชั่วโมงเพื่อแก้ไขปัญหาให้เสร็จสมบูรณ์

- เวิร์กโฟลว์ SharePoint 2010 หน่วงเวลาเมื่อเริ่มใช้งาน

    - ซึ่งจะเกิดขึ้นถ้าเวิร์กโฟลว์ถูกทริกเกอร์เป็นชุดใหญ่ (ตัวอย่างเช่น เมื่อมีการเพิ่มหลายรายการในครั้งเดียว)

    - เวิร์กโฟลว์ไม่ได้ออกแบบมาเพื่อเรียกใช้แบบเรียลไทม์ ดังนั้นการหน่วงเวลาจึงเกิดขึ้นตามลักษณะการดีไซน์

   -  ถ้าเวิร์กโฟลว์ซับซ้อน Extensible Object Markup Language (XRUP) การคอมไพล์อาจช้าได้ [ตรวจสอบ](https://support.microsoft.com//kb/3043697)บทความนี้

    - คุณควรลดความซับซ้อนของเวิร์กโฟลว์หรือออกแบบใหม่โดยใช้ชนิดแพลตฟอร์มเวิร์กโฟลว์ของ Microsoft SharePoint 2013

    - ถ้าประวัติเวิร์กโฟลว์ของคุณมีขนาดใหญ่ขึ้น คุณอาจต้องการล้างข้อมูลหรือสร้างรายการประวัติใหม่

        ข้อมูลเพิ่มเติม : [การล้างประวัติเวิร์กโฟลว์](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
ต้องการลองใช้ Microsoft Flow ใน SharePoint Online ใช่ไหม
- [สร้างโฟลว์](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint และ Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
