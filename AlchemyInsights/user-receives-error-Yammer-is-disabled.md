---
title: ผู้ใช้ได้รับข้อผิดพลาด AADSTS7000112 Yammerถูกปิดใช้งาน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: f2e23d63338ece5332ad4fd2b2d59021eb45d9bf32632d3cc23089c919d4e402
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971250"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>ผู้ใช้ได้รับข้อผิดพลาด AADSTS7000112 Yammerถูกปิดใช้งาน

ถ้าคุณได้รับข้อผิดพลาด "AADSTS7000112: แอปพลิเคชัน '00000005-0000-0ff1-ce00-0000000000' (Yammer) ถูกปิดใช้งาน" ปัญหาจะมีปัญหากับหลักบริการภายใน Azure AD ผู้ดูแลระบบอาจปิดใช้งานหลักของบริการเพื่อบล็อกYammerบริการ

ไม่แนะให้ปิดใช้งานบริการหลัก และอาจทําให้เกิดปัญหาเพิ่มเติมได้ For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

เมื่อต้องการแก้ไขปัญหานี้ในพอร์ทัล Azure และคืนค่าการเข้าถึงของผู้ใช้เพื่อYammer:

1.  เปิดAzure Active Directoryแล้วเลือก แอปพลิเคชัน **ขององค์กร****ภายใต้ จัดการ** ในบานหน้าต่างนําทางด้านซ้าย
3.  พิมพ์ **Office 365 Yammer** ในกล่องค้นหา แล้วเลือกชื่อแอปพลิเคชันเพื่อเปิดการตั้งค่า
4.  เลือก **คุณสมบัติ** ภายใต้ **จัดการ** ในบานหน้าต่างนําทางด้านซ้าย
5.  ตั้งค่า เปิดใช้งาน **ให้ผู้ใช้ลงชื่อเข้าใช้หรือไม่****เป็น** ใช่ **แล้วเลือก** บันทึก
6.  ลงชื่อเข้าใช้Yammerอีกครั้ง คุณอาจต้องล้างคุกกี้

หรือ เรียกใช้สั่ง PowerShell เพื่อตั้งค่า ดูข้อมูลเพิ่มเติมได้ที่ ข้อผิดพลาด["ขออภัย แต่เรามีปัญหาในการ](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)ลงชื่อเข้าใช้ให้คุณ" เมื่อคุณคลิกที่ไทล์Yammerใน Office 365 