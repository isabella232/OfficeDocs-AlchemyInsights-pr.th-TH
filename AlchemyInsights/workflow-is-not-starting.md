---
title: เวิร์กโฟลว์ไม่เริ่ม
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
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907757"
---
# <a name="workflow-is-not-starting"></a>เวิร์กโฟลว์ไม่เริ่ม

- SharePoint 2010 และ SharePoint 2013 เวิร์กโฟลว์ไม่เริ่มขึ้น

    - ถ้าเวิร์กโฟลว์ของคุณไม่เริ่มขึ้น อาจเป็นปัญหาการบริการชั่วคราวที่ผู้ใช้อาจพบความล่าช้าในความคืบหน้าของเวิร์กโฟลว์เป็นระยะๆ ตรวจสอบ [แดชบอร์ดสถานภาพ](https://admin.microsoft.com/AdminPortal/Home/servicehealth) บริการเพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่

    - หากคุณเห็นปัญหานี้เกิน 24 ชั่วโมง โปรดบันทึกตั๋วการสนับสนุน ในหลายกรณี เราแก้ไขปัญหาเรียบร้อยแล้ว โปรดให้เวลาเราอย่างน้อย 24 ชั่วโมงเพื่อแก้ไขปัญหาให้เสร็จสิ้น

- SharePoint 2010 เวิร์กโฟลว์ล่าช้าเมื่อเริ่มใช้งาน

    - ซึ่งจะเกิดขึ้นถ้าเวิร์กโฟลว์ถูกทริกเกอร์ในชุดใหญ่ (ตัวอย่างเช่น เมื่อมีการเพิ่มหลายรายการในครั้งเดียว)

    - เวิร์กโฟลว์ไม่ได้ออกแบบมาเพื่อใช้งานแบบเรียลไทม์ ดังนั้นการหน่วงเวลาจึงขึ้นอยู่กับลักษณะการดีไซน์

   -  ถ้าเวิร์กโฟลว์ซับซ้อน Extensible Object Markup Language (XDEN) การคอมไพล์อาจช้าได้ [ตรวจสอบ](https://support.microsoft.com//kb/3043697)บทความนี้

    - คุณควรลดความซับซ้อนของเวิร์กโฟลว์หรือออกแบบใหม่โดยใช้ชนิดแพลตฟอร์มเวิร์กโฟลว์ของ Microsoft SharePoint 2013

    - ถ้าประวัติเวิร์กโฟลว์ของคุณขยายใหญ่ขึ้น คุณอาจต้องการล้างข้อมูลหรือสร้างรายการประวัติใหม่

        ข้อมูลเพิ่มเติม : [ล้างประวัติเวิร์กโฟลว์](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
ต้องการMicrosoft Flowใน SharePoint Online ใช่ไหม
- [สร้างFlow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePointและFlow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
