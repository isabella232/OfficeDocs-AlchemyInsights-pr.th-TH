---
title: แก้ไขปัญหา - ไม่พบผู้ใช้ในไดเรกทอรี
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098189"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>แก้ไขปัญหา - ไม่พบผู้ใช้ในไดเรกทอรี

ถ้าผู้ใช้ได้รับข้อความแสดงข้อผิดพลาด "ไม่พบผู้ใช้" ในไดเรกทอรี โปรดลองอีกครั้งที่ ชนิดของปัญหาคือ ผู้ใช้ไม่อยู่ในไดเรกทอรี

คุณสามารถเสร็จสิ้นขั้นตอนต่อไปนี้เพื่อแก้ไขปัญหา

- ตรวจสอบให้แน่ใจว่าบัญชีที่ยอมรับคําเชิญทางอีเมลเป็นบัญชีเดียวกันกับที่ใช้เพื่อลงชื่อเข้าใช้ในภายหลัง Make sure the user is using the same account to accept the invite and sign into the site. 

ดูข้อมูลเพิ่มเติมได้ที่ วิธีการ[จัดการนามแฝงของบัญชี Microsoft เพื่อ </a> จัดการบัญชี Microsoft 365เข้าสู่ระบบ](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- เรียกดูแต่ละไซต์ที่ผู้ใช้ได้รับข้อผิดพลาด 

เพิ่ม "/_layouts/15/people.aspx/membershipgroupid=0" (ภายในเครื่องหมายอัญประกาศคู่) ไปยังส่วนท้ายของ URL ของไซต์ 

ตัวอย่าง: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0

- เลือกผู้ใช้จากรายการ

- คลิก **เอาสิทธิ์ของผู้ใช้** ออกจาก Ribbon 
-  เพิ่มผู้ใช้กลับและส่งการเชิญให้กับผู้ใช้อีกครั้ง

