---
title: ผู้ใช้ได้รับข้อผิดพลาด AADSTS7000112 Yammer ถูกปิดใช้งาน
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
ms.openlocfilehash: 3a3a1b531f3d775f7e5150ce86733a3012df8d0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796667"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>ผู้ใช้ได้รับข้อผิดพลาด AADSTS7000112 Yammer ถูกปิดใช้งาน

ถ้าคุณได้รับข้อผิดพลาด "AADSTS7000112: แอปพลิเคชัน ' 00000005-0000-0ff1-ce00-000000000000 ' (Yammer) ถูกปิดใช้งาน" ปัญหาที่มีอยู่ในบริการหลักภายใน Azure AD ผู้ดูแลระบบอาจปิดใช้งานหลักของบริการเพื่อบล็อกการเข้าถึง Yammer

การปิดใช้งานหลักของบริการไม่แนะนำและอาจทำให้เกิดปัญหาเพิ่มเติม สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการที่ได้รับการสนับสนุนเพื่อบล็อกการเข้าถึงของผู้ใช้ไปยัง Yammer ให้ดูที่[ปิดการเข้าถึง yammer สำหรับผู้ใช้ Microsoft ๓๖๕](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)  

เมื่อต้องการแก้ไขปัญหานี้ในพอร์ทัล Azure และคืนค่าการเข้าถึงของผู้ใช้ไปยัง Yammer:

1.  เปิดหน้าไดเรกทอรีที่ใช้งานอยู่ของ Azure แล้วเลือก **แอปพลิเคชันขององค์กร** ภายใต้ **จัดการ** ในบานหน้าต่างนำทางด้านซ้าย
3.  พิมพ์ **Office ๓๖๕ Yammer** ในกล่องค้นหาแล้วเลือกชื่อแอปพลิเคชันเพื่อเปิดการตั้งค่า
4.  เลือก **คุณสมบัติ** ภายใต้ **จัดการ** ในบานหน้าต่างนำทางด้านซ้าย
5.  ตั้งค่าของการ**เปิดใช้งานสำหรับผู้ใช้ในการลงชื่อเข้าใช้ใช่หรือไม่**เมื่อต้องการ**ใช่**แล้วเลือก**บันทึก**
6.  ลงชื่อเข้าใช้ Yammer อีกครั้ง คุณอาจจำเป็นต้องล้างคุกกี้

อีกวิธีหนึ่งคือเรียกใช้คำสั่ง PowerShell เพื่อตั้งค่า สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ "ขออภัยแต่เรากำลังมีปัญหาในการลงชื่อเข้าใช้คุณ" เมื่อคุณคลิกไทล์ Yammer ใน Office ๓๖๕](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365) 