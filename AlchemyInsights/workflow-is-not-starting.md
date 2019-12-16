---
title: เวิร์กโฟลว์ไม่ได้เริ่มต้น
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: cf7bd95e9a8f1d0842f0abcf82c758d649e80c0f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049356"
---
# <a name="workflow-is-not-starting"></a>เวิร์กโฟลว์ไม่ได้เริ่มต้น

- ไม่มีการเริ่มทำงาน SharePoint ๒๐๑๐และ SharePoint ๒๐๑๓เวิร์กโฟลว์

    - ถ้าเวิร์กโฟลว์ของคุณไม่ได้เริ่มต้นอาจมีปัญหาการบริการแบบถาวรที่ผู้ใช้อาจพบความล่าช้าเป็นระยะๆกับความคืบหน้าของเวิร์กโฟลว์ ตรวจสอบ[แดชบอร์ดความสมบูรณ์ของบริการ](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่

    - หากมีการผ่านมากกว่า24ชั่วโมงตั้งแต่แรกคุณเห็นปัญหานี้โปรดบันทึกตั๋วสนับสนุน ในหลายกรณีเรากำลังทำงานอยู่แล้วในการแก้ปัญหา กรุณาให้เราอย่างน้อย24ชั่วโมงในการดำเนินการแก้ปัญหา

- ลำดับงาน SharePoint ๒๐๑๐ที่ล่าช้าเมื่อเริ่มต้น

    - เหตุการณ์นี้เกิดขึ้นถ้าเวิร์กโฟลว์ถูกทริกเกอร์ในชุดงานขนาดใหญ่ (ตัวอย่างเช่นเมื่อมีการเพิ่มสินค้าหลายรายการพร้อมกัน)

    - เวิร์กโฟลว์ไม่ได้รับการออกแบบให้รันแบบเรียลไทม์เพื่อให้การหน่วงเวลาเป็นลักษณะการทำงานออกแบบ

   -  ถ้าเวิร์กโฟลว์เป็นภาษามาร์กอัปวัตถุ Extensible ที่ซับซ้อน (XMOL) การคอมไพล์สามารถทำได้ช้า ตรวจสอบบทความ[นี้](https://support.microsoft.com//kb/3043697)

    - คุณควรทำให้เวิร์กโฟลว์ของคุณง่ายขึ้นหรือออกแบบโดยใช้ชนิดแพลตฟอร์มของเวิร์กโฟลว์ Microsoft SharePoint ๒๐๑๓

    - ถ้าประวัติลำดับงานของคุณเติบโตขึ้นใหญ่คุณอาจต้องการล้างรายการหรือสร้างรายการประวัติใหม่

        ข้อมูลเพิ่มเติม:[ล้างประวัติลำดับงาน](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
ต้องการลองการไหลของ Microsoft ใน SharePoint แบบออนไลน์หรือไม่
- [สร้างโฟลว์](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint และการไหล](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


