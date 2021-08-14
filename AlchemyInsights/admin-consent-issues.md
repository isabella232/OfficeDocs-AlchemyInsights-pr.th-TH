---
title: ปัญหาความยินยอมของผู้ดูแลระบบ
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952592"
---
# <a name="admin-consent-issues"></a>ปัญหาความยินยอมของผู้ดูแลระบบ

1. เปิดใช้งานเวิร์กโฟลว์ [ความยินยอมของผู้ดูแลระบบ](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) เพื่ออนุญาตให้ผู้ใช้ร้องขอการอนุมัติจากผู้ดูแลระบบได้โดยตรงจากหน้าจอความยินยอม

1. ถ้าคุณหรือผู้ใช้แอปพลิเคชันของคุณพบข้อผิดพลาดที่ไม่คาดคิดในระหว่างกระบวนการยินยอม ให้ดูบทความนี้เพื่อดูขั้นตอนการแก้ไขปัญหา: ข้อผิดพลาดที่ไม่คาดคิดเมื่อได้รับความยินยอม [จาก](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)แอปพลิเคชัน

1. เรียนรู้เพิ่มเติมเกี่ยวกับ[ความยินยอมของผู้ดูแลระบบแพลตฟอร์มข้อมูลประจําตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)วิธีการงาน[พร้อมท์](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)การยินยอม และวิธีการประเมินการร้องขอความยินยอมของผู้ดูแลระบบ[ทั้ง](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)ผู้เช่า

1. แอปพลิเคชันที่รวมแพลตฟอร์มข้อมูลประจําตัวของ Microsoftติดตามรูปแบบการอนุญาตที่ให้ผู้ใช้และผู้ดูแลระบบควบคุมวิธีเข้าถึงข้อมูล การปรับใช้รูปแบบการอนุญาตได้รับการอัปเดตบนจุดสิ้นสุด แพลตฟอร์มข้อมูลประจําตัวของ Microsoft และจะเปลี่ยนวิธีที่แอปต้องโต้ตอบกับแพลตฟอร์มข้อมูลประจําตัวของ Microsoft ดู[สิทธิ์และความยินยอมในแพลตฟอร์มข้อมูลประจําตัวของ Microsoftปลายทาง](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)ของกลุ่มเพื่อดูภาพรวมของรูปแบบการอนุญาตนี้ รวมถึงขอบเขต สิทธิ์ และความยินยอม