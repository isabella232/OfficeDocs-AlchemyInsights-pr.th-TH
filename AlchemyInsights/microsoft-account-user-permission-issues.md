---
title: สร้าง และใช้กล่องจดหมายที่ใช้ร่วมกัน
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762419"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>แก้ไขปัญหา - ไม่พบในไดเรกทอรีของผู้ใช้

ถ้าผู้ใช้ได้รับข้อผิดพลาดข้อความ "ไม่พบผู้ใช้" ในไดเรกทอรี โปรดลองอีกครั้ง ที่ชนิดการตัดสินค้าจากคลังที่ผู้ใช้ไม่มีไดเรกทอรี

ขั้นตอนต่อไปนี้สามารถให้สมบูรณ์เพื่อแก้ปัญหา

- ให้แน่ใจว่าบัญชีที่ยอมรับการเชิญทางอีเมลเป็นบัญชีเดียวกับที่ใช้เข้าสู่ระบบในภายหลัง ตรวจสอบให้แน่ใจว่า ผู้ใช้ที่กำลังใช้บัญชีเดียวกันเพื่อยอมรับการเชิญ และเซ็นชื่อลงในไซต์ 

สำหรับข้อมูลเพิ่มเติม ดู[วิธีการจัดการนามแฝงสำหรับบัญชีของคุณ Microsoft</a>การจัดการการเข้าสู่ระบบ Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- เรียกดูไซต์แต่ละผู้ใช้ได้รับข้อผิดพลาด 

เพิ่ม " / _layouts/15/people.aspx/membershipgroupid=0 " (ภายในอัญประกาศ) ลงในส่วนท้ายของ URL ของไซต์ 

ตัวอย่าง: _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 https://_lT

- เลือกผู้ใช้จากรายการ

- คลิก**เอาออกสิทธิ์ของผู้ใช้**จาก Ribbon 
-  เพิ่มผู้ใช้กลับ และส่งการเชิญไปยังผู้ใช้

