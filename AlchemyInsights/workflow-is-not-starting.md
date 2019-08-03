---
title: ไม่สามารถเริ่มต้นเวิร์กโฟลว์
ms.author: efrene
author: efrene
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
ms.openlocfilehash: efd17c302ae6d857207e87e94d74d3794e94a83a
ms.sourcegitcommit: 204be4a6ae03700b75eae6b09b4e9ab283089fbf
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/03/2019
ms.locfileid: "36171819"
---
# <a name="workflow-is-not-starting"></a>ไม่สามารถเริ่มต้นเวิร์กโฟลว์

- ลำดับงาน SharePoint 2010 และ SharePoint 2013 จะไม่เริ่มต้น

    ถ้าไม่สามารถเริ่มต้นเวิร์กโฟลว์ของคุณ อาจมีปัญหากับบริการชั่วคราวซึ่งผู้ใช้อาจพบความล่าช้าเป็นระยะ ๆ ด้วยความคืบหน้าของลำดับงาน ตรวจสอบ[ความสมบูรณ์ของแดชบอร์ดบริการซึ่ง](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth)เมื่อต้องการดูถ้าองค์กรของคุณได้รับผลกระทบ

    ถ้ามากกว่า 24 ชั่วโมงได้ตั้งแต่คุณเห็นปัญหานี้ขั้นแรก โปรดเข้าสู่ระบบ ticket สนับสนุน ในหลายกรณี เรากำลังทำงานอยู่ในโซลูชัน โปรดให้กับเราอย่างน้อย 24 ชั่วโมงในการแก้ไขปัญหาการทำให้เสร็จสมบูรณ์

- เวิร์กโฟลว์ SharePoint 2010 ล่าช้าในการเริ่มต้นเท่านั้น

    เหตุการณ์นี้เกิดขึ้นถ้าเวิร์กโฟลว์จะถูกทริกเกอร์เป็นชุดงานขนาดใหญ่ (ตัวอย่างเช่น เมื่อหลายรายการบวกในคราวเดียวกัน)

    เวิร์กโฟลว์ไม่ได้ออกแบบมาเพื่อทำงานแบบเรียลไทม์ ดังนั้นการเลื่อนเวลาเป็นลักษณะการทำงานด้วยการออกแบบ

    ถ้าเวิร์กโฟลว์ ซับซ้อน Extensible วัตถุมาร์กอัปภาษา (XMOL), คอมไพล์สามารถทำได้ล่าช้า ตรวจสอบบทความ[นี้](https://support.microsoft.com/en-us/kb/3043697)

    คุณควรทำเวิร์กโฟลว์ หรือออกแบบโดยใช้ชนิดของแพลตฟอร์มเวิร์กโฟลว์ 2013 ของ Microsoft SharePoint

    นอกจากนี้ ถ้าประวัติเวิร์กโฟลว์ของคุณขยายใหญ่จน คุณอาจต้องการกำจัดสินค้า หรือสร้างรายการประวัติใหม่

    หากต้องการข้อมูลเพิ่มเติม:[ล้างประวัติลำดับงาน](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
ต้องการลองขั้นตอน Micrsoft ใน SharePoint แบบออนไลน์หรือไม่
- [สร้างขั้นตอน](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint และขั้นตอน](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


