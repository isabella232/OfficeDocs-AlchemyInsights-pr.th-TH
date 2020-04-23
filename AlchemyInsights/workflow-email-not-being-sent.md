---
title: ไม่มีการส่งอีเมลลําดับงาน
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
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766152"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>ไม่มีการส่งอีเมลลําดับงานสําหรับรายการหรือไลบรารี SharePoint

1. อีเมลจากเวิร์กโฟลว์จะไม่ถูกส่งไปยังผู้ใช้ทั้งหมดหรือเฉพาะผู้ใช้ที่ระบุ หรือ**คุณเห็นข้อผิดพลาด ตรวจสอบให้แน่ใจว่าอีเมลมีผู้รับที่ถูกต้อง**

    ตรวจสอบว่าผู้ใช้ที่มีอยู่ในกลุ่มสิทธิ์**บุคคลทั้งหมด**(รายการข้อมูลผู้ใช้) สําหรับไซต์คอลเลกชันนั้นหรือไม่  ตัวอย่าง URL โดยตรง<tenant>:<sitename>https:// .sharepoint.com/sites/ / _layouts / 15 / people.aspx? สมาชิกกลุ่มId = 0

    - ถ้าผู้ใช้ไม่มี อยู่ ตรวจสอบให้แน่ใจว่า ผู้ใช้ได้ลงชื่อเข้าใช้ในเพจ 
    - ถ้าเป็นผู้ใช้ภายนอก ให้ตรวจสอบว่าคําเชิญของพวกเขาได้รับการยอมรับแล้ว
    - ถ้าผู้ใช้ไม่มีอยู่ในกลุ่มสิทธิ์
    - ถ้าไม่ได้ตั้งค่าที่อยู่อีเมลของผู้ใช้ที่นี่ แล้วสร้างการแจ้งเตือนตัวอย่างสําหรับผู้ใช้ที่บังคับให้ซิงค์ของบัญชีผู้ใช้นั้นจากโปรไฟล์ผู้ใช้ของ SharePoint ไปยังไซต์คอลเลกชันนี้
 
2. อีเมลจากเวิร์กโฟลว์จะถูกส่งไปยังผู้ดูแลไซต์คอลเลกชัน แต่ไม่ให้ผู้ใช้อื่น เห็นข้อผิดพลาด HTTP Forbidden เป็น**<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.SendEmail**
 

    ดู[การเข้าถึงถูกปฏิเสธเมื่อคุณส่งอีเมลไปยังกลุ่ม SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    นอกจากนี้ ตรวจสอบว่า ผู้ใช้สิทธิ์**lockdown**จํากัดสิทธิ์ผู้ใช้คุณลักษณะชุดเก็บรวบรวมไซต์


## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
ต้องการลอง Microsoft ไหลใน SharePoint แบบออนไลน์หรือไม่
- [สร้างโฟลว์](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint และโฟลว์](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


