---
title: ไม่มีการส่งอีเมลการเวิร์กโฟลว์
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270691"
---
# <a name="workflow-email-is-not-being-sent"></a>ไม่มีการส่งอีเมลการเวิร์กโฟลว์

1. อีเมลจากเวิร์กโฟลว์จะไม่ถูกส่งถึงผู้ใช้ทั้งหมดหรือผู้ใช้ที่ระบุเท่านั้น หรือคุณเห็นข้อความอีเม**ข้อผิดพลาดไม่สามารถส่ง ตรวจสอบว่า อีเมลที่มีผู้รับที่ถูกต้อง**

    ตรวจสอบว่ามีผู้ใช้ในกลุ่มสิทธิ์**ทุกคน**(รายการข้อมูลผู้ใช้) สำหรับไซต์คอลเลกชัน  ตัวอย่าง URL โดยตรง: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx หรือไม่ MembershipGroupId = 0

    - ถ้าผู้ใช้ไม่มีอยู่ ทำให้แน่ใจว่า ผู้ใช้มีการเซ็นชื่อลงในเพจ 
    - ถ้าคุณเป็นผู้ใช้ภายนอก โปรดตรวจสอบให้แน่ใจว่า มีการยอมรับการเชิญ
    - ถ้ามีผู้ใช้ในกลุ่มสิทธิ์ ทำให้แน่ใจว่า อยู่อีเมลที่ถูกต้อง
    - ถ้าอยู่อีเมลของผู้ใช้ถูกกำหนดที่นี่ สร้างตัวอย่างข้อความแจ้งเตือนสำหรับผู้ใช้ซึ่งเป็นบังคับการซิงค์ของบัญชีผู้ใช้นั้นจากโพรไฟล์ผู้ใช้ของ SharePoint เพื่อเก็บรวบรวมไซต์นี้
 
2. อีเมลจากเวิร์กโฟลว์จะถูกส่ง ไปที่ผู้ดูแลชุดเก็บรวบรวมไซต์ แต่ไม่ใช่ กับผู้ใช้รายอื่น และดูข้อผิดพลาด**อนุญาตให้ใช้ HTTP <spam> <spam> ** <spam> <spam>
 

    ดูการ[เข้าถึงถูกปฏิเสธเมื่อส่งอีเมลถึงกลุ่ม](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups)

    ตรวจสอบด้วย ว่า คุณลักษณะ**โหมด lockdown สิทธิ์ของผู้ใช้ถูกจำกัดการเข้าถึง**ไซต์คอลเลกชันไม่ได้ใช้งาน


## <a name="related-topics"></a>หัวข้อที่เกี่ยวข้อง
ต้องการลองกระแส Microsoft ใน SharePoint แบบออนไลน์หรือไม่
- [สร้างขั้นตอน](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint และขั้นตอน](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


