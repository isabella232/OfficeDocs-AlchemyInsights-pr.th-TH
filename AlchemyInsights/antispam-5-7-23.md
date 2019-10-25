---
title: การป้องกันสแปม-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682326"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>แก้ไขปัญหาการส่งเมล์สำหรับรหัสข้อผิดพลาด5.7.23

ตรวจสอบระเบียน SPF DNS สำหรับโดเมนของคุณในตัวตรวจสอบระเบียน SPF หรือ DNS ที่พร้อมใช้งานสาธารณะบนเว็บ

ตรวจสอบว่าข้อความขาออกไม่ได้ระบุว่าเป็นสแปมโดย Office ๓๖๕และกำหนดเส้นทางผ่าน[กลุ่มการจัดส่งความเสี่ยงสูง](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages) ข้อความในพูลการจัดส่งความเสี่ยงสูงจะไม่ผ่านการตรวจสอบ SPF และดังนั้นจึงจะไม่ได้รับการอนุญาตจากองค์กรของคุณ

ถ้าปัญหายังคงมีอยู่คุณอาจต้องติดต่อผู้ดูแลของโฮสต์จดหมายที่คุณกำลังพยายามที่จะส่งทางเมล จดบันทึกข้อผิดพลาดภายนอกโดยละเอียดที่มีอยู่ในข้อความตีกลับ  การสนับสนุน Office ๓๖๕อาจไม่สามารถช่วยเหลือเพิ่มเติมได้