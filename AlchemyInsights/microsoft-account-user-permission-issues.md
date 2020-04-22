---
title: แก้ไขปัญหา - ไม่พบผู้ใช้ในไดเรกทอรี
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702757"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>แก้ไขปัญหา - ไม่พบผู้ใช้ในไดเรกทอรี

หากผู้ใช้ได้รับข้อความแสดงข้อผิดพลาด "ไม่พบผู้ใช้" ในไดเรกทอรี โปรดลองอีกครั้งที่ประเภทปัญหาคือ ผู้ใช้ไม่ได้อยู่ในไดเรกทอรี

ขั้นตอนต่อไปนี้สามารถเสร็จสมบูรณ์เพื่อแก้ไขปัญหา

- ตรวจสอบให้แน่ใจว่าบัญชีที่ยอมรับคําเชิญทางอีเมลเป็นบัญชีเดียวกับที่ใช้ในการลงชื่อเข้าใช้ในภายหลัง ตรวจสอบว่าผู้ใช้ใช้บัญชีเดียวกันเพื่อยอมรับคําเชิญและลงชื่อเข้าใช้ไซต์ 

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[วิธีจัดการนามแฝงสําหรับบัญชี</a>Microsoft ของคุณเพื่อจัดการการเข้าสู่ระบบ Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- เรียกดูแต่ละไซต์ซึ่งผู้ใช้ได้รับข้อผิดพลาด 

เพิ่ม "/_layouts/15/people.aspx/membershipgroupid=0" (ภายในเครื่องหมายอัญประกาศคู่) ไปยังส่วนท้ายของ URL ของไซต์ 

ตัวอย่าง: https://<"contoso">.sharepoint.com/_layouts 15/people.aspx/สมาชิกกลุ่มId =0

- เลือกผู้ใช้จากรายการ

- คลิก**เอาสิทธิ์ของผู้ใช้**ออกจาก Ribbon 
-  เพิ่มกลับผู้ใช้และส่งคําเชิญไปยังผู้ใช้

