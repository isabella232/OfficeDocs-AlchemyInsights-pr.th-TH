---
title: ไม่มีการส่งอีเมลของเวิร์กโฟลว์
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
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749028"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>ไม่มีการส่งอีเมลของเวิร์กโฟลว์สำหรับรายการหรือไลบรารี SharePoint

1. อีเมลจากเวิร์กโฟลว์จะไม่ถูกส่งไปยังผู้ใช้ทั้งหมดหรือเฉพาะผู้ใช้ที่ระบุเท่านั้นหรือคุณเห็นข้อผิดพลาด**ที่ไม่สามารถส่งข้อความอีเมลได้ตรวจสอบให้แน่ใจว่าอีเมลมีผู้รับที่ถูกต้อง**

    ตรวจสอบว่าผู้ใช้มีอยู่ในกลุ่มสิทธิ์ของ **บุคคลทั้งหมด** (รายการข้อมูลผู้ใช้) สำหรับไซต์คอลเลกชันนั้นหรือไม่  ตัวอย่าง URL โดยตรง: https:// <tenant> sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx MembershipGroupId = 0

    - ถ้าไม่มีผู้ใช้ตรวจสอบให้แน่ใจว่าผู้ใช้ลงชื่อเข้าใช้หน้า 
    - ถ้าเป็นผู้ใช้ภายนอกตรวจสอบให้แน่ใจว่าการเชิญของพวกเขาได้รับการยอมรับแล้ว
    - ถ้าผู้ใช้มีอยู่ในกลุ่มสิทธิ์ตรวจสอบให้แน่ใจว่าที่อยู่อีเมลนั้นถูกต้อง
    - ถ้าที่อยู่อีเมลของผู้ใช้ไม่ได้ตั้งค่าที่นี่จากนั้นสร้างการแจ้งเตือนตัวอย่างสำหรับผู้ใช้ที่บังคับให้มีการซิงค์บัญชีผู้ใช้นั้นจากโปรไฟล์ผู้ใช้ของ SharePoint ไปยังไซต์คอลเลกชันนี้
 
2. อีเมลจากเวิร์กโฟลว์จะถูกส่งไปยังผู้ดูแลไซต์คอลเลกชันแต่ไม่ใช่ผู้ใช้อื่นและดูข้อผิดพลาด**HTTP ที่ห้ามใช้<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.sendemail**
 

    ให้ดูที่[การเข้าถึงถูกปฏิเสธเมื่อคุณส่งอีเมลไปยังกลุ่ม SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    นอกจากนี้ให้ตรวจสอบว่าฟีเจอร์ไซต์คอลเลกชัน **สิทธิ์ของผู้ใช้ที่มีสิทธิ์การเข้าถึงแบบจำกัด** ไม่ได้ใช้งานอยู่


## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
ต้องการลองใช้ Microsoft Flow ใน SharePoint Online หรือไม่
- [สร้างขั้นตอน](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint และการไหล](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


