---
title: แก้ไขปัญหา-ไม่พบผู้ใช้ในไดเรกทอรี
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054829"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>แก้ไขปัญหา-ไม่พบผู้ใช้ในไดเรกทอรี

ถ้าผู้ใช้ได้รับข้อความข้อผิดพลาด "ผู้ใช้ไม่พบ" ในไดเรกทอรีโปรดลองอีกครั้งที่ชนิดของปัญหาเป็นผู้ใช้ไม่ได้อยู่ในไดเรกทอรี

ขั้นตอนต่อไปนี้สามารถทำให้เสร็จสมบูรณ์เพื่อแก้ไขปัญหา

- ตรวจสอบให้แน่ใจว่าบัญชีที่ยอมรับการเชิญทางเมลเป็นบัญชีเดียวกันกับที่ใช้ในการเข้าสู่ระบบในภายหลัง ตรวจสอบให้แน่ใจว่าผู้ใช้ใช้บัญชีเดียวกันเพื่อยอมรับการเชิญและลงชื่อเข้าใช้เว็บไซต์ 

สำหรับข้อมูลเพิ่มเติมให้ดู[วิธีการจัดการนามแฝงสำหรับบัญชี</a> Microsoft ของคุณเพื่อจัดการ Office ๓๖๕เข้าสู่ระบบ](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- เรียกดูไปยังแต่ละไซต์ที่ผู้ใช้ได้รับข้อผิดพลาด 

เพิ่ม "/_layouts/15/people.aspx/membershipgroupid = 0" (ภายในอัญประกาศคู่) ไปยังจุดสิ้นสุดของ URL ของไซต์ 

ตัวอย่าง: https://< "contoso" > sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0

- เลือกผู้ใช้จากรายการ

- คลิ**กเอาออกสิทธิ์ของผู้ใช้**จาก Ribbon 
-  เพิ่มผู้ใช้และส่งการเชิญไปยังผู้ใช้อีกครั้ง

