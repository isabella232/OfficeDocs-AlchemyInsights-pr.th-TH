---
title: เวิร์กโฟลว์ไม่ได้เริ่มต้น
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766116"
---
# <a name="workflow-is-not-starting"></a>เวิร์กโฟลว์ไม่ได้เริ่มต้น

- เวิร์กโฟลว์ SharePoint 2010 และ SharePoint 2013 จะไม่เริ่มทํางาน

    - ถ้าเวิร์กโฟลว์ของคุณไม่ได้เริ่มต้น อาจมีปัญหาการบริการชั่วคราวซึ่งผู้ใช้อาจพบความล่าช้าเป็นระยะ ๆ กับความคืบหน้าของเวิร์กโฟลว์ ตรวจสอบ[แดชบอร์ดสถานภาพบริการ](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่

    - หากผ่านเกิน 24 ชั่วโมงตั้งแต่เห็นปัญหานี้ครั้งแรกโปรดเข้าสู่ระบบตั๋วสนับสนุน ในหลายกรณีเรากําลังทํางานเกี่ยวกับโซลูชันอยู่แล้ว โปรดให้เราอย่างน้อย 24 ชั่วโมงเพื่อแก้ปัญหา

- เวิร์กโฟลว์ SharePoint 2010 ล่าช้าเมื่อเริ่มต้น

    - เหตุการณ์นี้เกิดขึ้นถ้าเวิร์กโฟลว์จะถูกทริกเกอร์ในชุดงานขนาดใหญ่ (ตัวอย่างเช่น เมื่อมีหลายรายการถูกเพิ่มในครั้งเดียว)

    - เวิร์กโฟลว์ไม่ได้ออกแบบมาเพื่อทํางานแบบเรียลไทม์ ดังนั้นความล่าช้าคือลักษณะการทํางานการออกแบบ

   -  ถ้ากระแสงานเป็นภาษามาร์กอัปวัตถุ Extensible ซับซ้อน (XMOL), การคอมไพล์สามารถช้า ตรวจสอบ[บทความนี้](https://support.microsoft.com//kb/3043697)

    - คุณควรทําให้เวิร์กโฟลว์ง่ายขึ้นหรือออกแบบใหม่โดยใช้ชนิดแพลตฟอร์มเวิร์กโฟลว์ของ Microsoft SharePoint 2013

    - ถ้าประวัติเวิร์กโฟลว์ของคุณมีขนาดใหญ่ขึ้นคุณอาจต้องการล้างรายการหรือสร้างรายการประวัติใหม่

        ข้อมูลเพิ่มเติม :[ประวัติเวิร์กโฟลว์การล้างข้อมูล](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
ต้องการลอง Microsoft ไหลใน SharePoint แบบออนไลน์หรือไม่
- [สร้างโฟลว์](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint และโฟลว์](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


