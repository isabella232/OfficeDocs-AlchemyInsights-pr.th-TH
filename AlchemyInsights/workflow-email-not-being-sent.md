---
title: ไม่มีการส่ง email ของลำดับงาน
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049392"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>ไม่มีการส่งเมลของลำดับงานสำหรับรายการหรือไลบรารี SharePoint

1. ไม่มีส่งจดหมายจากเวิร์กโฟลว์ไปยังผู้ใช้ทั้งหมดหรือเฉพาะผู้ใช้หรือคุณเห็นข้อผิดพลาด**ที่ไม่สามารถส่งข้อความทาง e-mail ตรวจสอบให้แน่ใจว่า e-mail มีผู้รับที่ถูกต้อง**

    ตรวจสอบว่าผู้ใช้มีอยู่ในกลุ่มสิทธิ์**คนทั้งหมด**(รายการข้อมูลผู้ใช้) สำหรับไซต์คอลเลกชันนั้น  ตัวอย่าง URL โดยตรง<tenant>: https://<sitename>/_layouts/15/sharepoint.com/sites/? MembershipGroupId = 0

    - ถ้าผู้ใช้ไม่มีอยู่โปรดตรวจสอบให้แน่ใจว่าผู้ใช้ที่มีการลงชื่อเข้าสู่หน้าเว็บ 
    - หากเป็นผู้ใช้ภายนอกโปรดตรวจสอบให้แน่ใจว่าได้ยอมรับคำเชิญของพวกเขาแล้ว
    - ถ้าผู้ใช้ไม่มีอยู่ในกลุ่มสิทธิ์โปรดตรวจสอบให้แน่ใจว่าที่อยู่ของเมลไม่ถูกต้อง
    - ถ้าไม่ได้ตั้งค่าที่อยู่ e-mail ของผู้ใช้ที่นี่แล้วสร้างการแจ้งเตือนตัวอย่างสำหรับผู้ใช้ที่บังคับให้ซิงค์ของบัญชีผู้ใช้นั้นจากโปรไฟล์ผู้ใช้ของ SharePoint ไปยังไซต์คอลเลกชันนี้
 
2. มีส่งจดหมายจากเวิร์กโฟลว์ไปยังผู้ดูแลชุดเก็บรวบรวมไซต์แต่ไม่ได้ให้กับคนอื่นและดูข้อผิดพลาด**HTTP ต้องห้ามไปยัง<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.sendemail**
 

    ดูการ[เข้าถึงถูกปฏิเสธเมื่อคุณส่งเมลไปยังกลุ่ม SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    นอกจากนี้ให้ตรวจสอบว่าการ**เข้าถึงแบบจำกัดสิทธิ์ผู้ใช้โหมด lockdown**ไซต์คอลเลกชันไม่ทำงาน


## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
ต้องการลองการไหลของ Microsoft ใน SharePoint แบบออนไลน์หรือไม่
- [สร้างโฟลว์](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint และการไหล](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


