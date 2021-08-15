---
title: เรียกคืนหรือแทนที่ข้อความอีเมล
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024405"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>เรียกคืนหรือแทนที่ข้อความอีเมลในMicrosoft 365

- คุณสามารถ **เรียกคืนข้อความที่ส่งไปยังบุคคลในองค์กรของคุณ** เท่านั้น ตัวอย่างเช่น ถ้าข้อความถูกส่งไปยังที่อยู่ Gmail คุณไม่สามารถเรียกคืนได้
- คุณสามารถ **เรียกคืนข้อความที่ส่งจากOutlookไปยังพีซี** เท่านั้น ถ้าผู้ใช้ส่งข้อความโดยใช้ข้อความOutlook for Mac Outlook บนเว็บข้อความ คุณไม่สามารถเรียกคืนได้
- ในฐานะผู้ดูแลระบบผู้เช่า คุณสามารถ **เรียกคืนข้อความในนามของผู้ใช้ได้โดยใช้ PowerShell** (ดูข้อมูลเพิ่มเติมที่: [ค้นหาและลบข้อความอีเมล](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization))
- คุณไม่สามารถเรียกคืนข้อความจากศูนย์การจัดการได้ เลื่อนลงไปที่ "ค้นหาและลบข้อความอีเมลในองค์กรของคุณ" เพื่อดูข้อมูลเพิ่มเติม

**เรียกคืนหรือแทนที่ข้อความอีเมลที่คุณส่ง**

1. ในบานหน้าต่างโฟลเดอร์ทางด้านซ้ายของOutlook จดหมาย ให้เลือกโฟลเดอร์ รายการที่ถูกส่ง
2. เปิดข้อความที่คุณต้องการเรียกคืน คุณต้องดับเบิลคลิกเพื่อเปิดข้อความ การเลือกข้อความเพื่อให้ข้อความนั้นปรากฏในบานหน้าต่างการอ่านจะไม่อนุญาตให้คุณเรียกคืนข้อความได้
3. จากแท็บ ข้อความ ให้เลือก การ **เรียกคืน**  >  **ข้อความ** นี้
4. เลือก **ลบสเนาที่ยังไม่ได้อ่านของข้อความ****นี้ หรือ ลบสเนาที่ยังไม่ได้อ่านและแทนที่** ด้วยข้อความใหม่ **จากนั้นเลือก** ตกลง
5. ถ้าคุณส่งข้อความทดแทน ให้เขียนข้อความ **จากนั้นเลือก** ส่ง
6. การเรียกคืนข้อความจะสเร็จหรือล้มเหลวจะขึ้นอยู่กับการตั้งค่าของOutlookผู้รับ

For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***เมื่อต้องการค้นหาและลบข้อความอีเมลใน*** องค์กรของคุณ วิธีที่ง่ายที่สุดคือถ้าคุณเป็นผู้ดูแลระบบส่วนกลาง ถ้าคุณไม่ใช่ผู้ดูแลระบบส่วนกลาง บัญชีของคุณต้องถูกเพิ่มลงในกลุ่มบทบาทตัวจัดการ eDiscovery หรือบทบาทการจัดการการค้นหาการปฏิบัติตามข้อบังคับ เมื่อต้องการลบข้อความ คุณจะต้องเข้าร่วมกลุ่มบทบาทการจัดการองค์กรหรือบทบาทการจัดการการค้นหาและล้าง สิทธิ์ในบทบาทเหล่านี้จะถูกมอบหมาย[ในศูนย์&การปฏิบัติตามนโยบาย](https://protection.office.com/)

1. [สร้างการค้นหา](https://docs.microsoft.com/microsoft-365/compliance/content-search) เนื้อหาเพื่อค้นหาข้อความที่จะลบ
2. [เชื่อมต่อศูนย์การรักษา&การปฏิบัติตามนโยบายของ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

ถ้าคุณใช้ MFA (การรับรองความถูกต้องแบบหลายปัจจัย) ให้ดู เชื่อมต่อ Microsoft 365ศูนย์&[การปฏิบัติตามนโยบายของ PowerShell โดยใช้การรับรองความถูกต้องแบบหลาย](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)ปัจจัย
