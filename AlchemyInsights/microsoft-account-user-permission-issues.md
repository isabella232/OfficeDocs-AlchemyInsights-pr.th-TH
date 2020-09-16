---
title: แก้ไขปัญหา-ผู้ใช้ที่ไม่พบในไดเรกทอรี
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725426"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>แก้ไขปัญหา-ผู้ใช้ที่ไม่พบในไดเรกทอรี

ถ้าผู้ใช้ได้รับข้อความแสดงข้อผิดพลาด "ไม่พบผู้ใช้" ในไดเรกทอรีโปรดลองอีกครั้งว่าชนิดของปัญหาคือผู้ใช้ที่ไม่ได้อยู่ในไดเรกทอรี

ขั้นตอนต่อไปนี้สามารถทำให้เสร็จสมบูรณ์ได้เพื่อแก้ไขปัญหา

- ตรวจสอบให้แน่ใจว่าบัญชีผู้ใช้ที่ยอมรับคำเชิญทางอีเมลเป็นบัญชีผู้ใช้เดียวกันกับที่ใช้ในการลงชื่อเข้าใช้ในภายหลัง ตรวจสอบให้แน่ใจว่าผู้ใช้กำลังใช้บัญชีผู้ใช้เดียวกันเพื่อยอมรับการเชิญและลงชื่อเข้าใช้ไซต์ 

สำหรับข้อมูลเพิ่มเติมให้ดู[ที่วิธีการจัดการนามแฝงสำหรับบัญชี microsoft ของคุณ </a> เพื่อจัดการการเข้าสู่ระบบ microsoft ๓๖๕](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- เรียกดูไซต์แต่ละไซต์ที่ผู้ใช้ได้รับข้อผิดพลาด 

เพิ่ม "/_layouts/15/people.aspx/membershipgroupid = 0" (ภายในเครื่องหมายอัญประกาศคู่) จนถึงจุดสิ้นสุดของ URL ของไซต์ 

ตัวอย่าง: https://< "contoso" > sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0

- เลือกผู้ใช้จากรายการ

- คลิก **เอาสิทธิ์ของผู้ใช้ออก** จาก Ribbon 
-  เพิ่มกลับผู้ใช้และส่งการเชิญไปยังผู้ใช้อีกครั้ง

