---
title: อีเมลเวิร์กโฟลว์จะไม่ถูกส่ง
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
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072539"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>อีเมลเวิร์กโฟลว์จะไม่ถูกส่งไปSharePointรายการหรือไลบรารี

1. อีเมลจากเวิร์กโฟลว์จะไม่ถูกส่งไปยังผู้ใช้ทั้งหมด หรือเฉพาะผู้ใช้ที่ระบุ หรือคุณเห็นข้อผิดพลาด ไม่สามารถส่งข้อความอีเมลได้ **ตรวจสอบให้แน่ใจว่าอีเมลมีผู้รับ** ที่ถูกต้อง

    ตรวจสอบว่าผู้ใช้อยู่ในกลุ่มสิทธิ์ **บุคคลทั้งหมด** (รายการข้อมูลผู้ใช้) ของไซต์คอลเลกชันนั้นหรือไม่  ตัวอย่าง URL โดยตรง: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx MembershipGroupId=0

    - ถ้าไม่มีผู้ใช้อยู่ ให้ตรวจสอบให้แน่ใจว่าผู้ใช้ได้ลงชื่อเข้าใช้เพจแล้ว 
    - If it is an external user, make sure that their invitation has been accepted.
    - ถ้าผู้ใช้อยู่ในกลุ่มสิทธิ์ ตรวจสอบให้แน่ใจว่าที่อยู่อีเมลถูกต้อง
    - ถ้าที่อยู่อีเมลของผู้ใช้ไม่ได้ตั้งค่าไว้ที่นี่ ให้สร้างตัวอย่างการแจ้งเตือนของผู้ใช้ซึ่งบังคับให้ซิงค์บัญชีผู้ใช้นั้นจาก โปรไฟล์ผู้ใช้ SharePointไปยังไซต์คอลเลกชันนี้
 
2. อีเมลจากเวิร์กโฟลว์จะถูกส่งไปยังผู้ดูแลไซต์คอลเลกชัน แต่ไม่ใช่กับผู้ใช้อื่นและดูข้อผิดพลาด **HTTP Forbidden ไปยัง <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendAmail**
 

    ดู[การเข้าถึงถูกปฏิเสธ เมื่อคุณส่งอีเมลไปยังSharePointของคุณ](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    นอกจากนี้ ให้ตรวจสอบว่าฟีเจอร์ **โหมดการจํากัดสิทธิ์การเข้าถึงของผู้ใช้ที่** จํากัดการเข้าถึงของไซต์คอลเลกชันไม่ได้ใช้งานอยู่


## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
ต้องการMicrosoft Flowใน SharePoint Online ใช่ไหม
- [สร้างFlow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePointและFlow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


