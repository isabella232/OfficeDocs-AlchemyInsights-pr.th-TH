---
title: ปัญหาเกี่ยวกับความยินยอมของผู้ดูแลระบบ
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
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901514"
---
# <a name="admin-consent-issues"></a>ปัญหาเกี่ยวกับความยินยอมของผู้ดูแลระบบ

1. เปิดใช้ [งานเวิร์กโฟลว์ความยินยอมของผู้ดูแลระบบ](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) เพื่ออนุญาตให้ผู้ใช้ร้องขอการอนุมัติจากผู้ดูแลระบบโดยตรงจากหน้าจอความยินยอม

1. ถ้าคุณหรือผู้ใช้ของแอปพลิเคชันของคุณเห็นข้อผิดพลาดที่ไม่คาดคิดในระหว่างกระบวนการยินยอมให้ดูบทความนี้สำหรับขั้นตอนการแก้ไขปัญหา:[ข้อผิดพลาดที่ไม่คาดคิดเมื่อทำการยินยอมให้กับแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. เรียนรู้เพิ่มเติมเกี่ยวกับ[ความยินยอมของผู้ดูแลระบบบนแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)วิธีการทำงานของ[พร้อมท์การยินยอม](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)และวิธีการ[ประเมินคำขอความยินยอมของผู้ดูแลระบบสำหรับผู้เช่า](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. แอปพลิเคชันที่รวมเข้ากับ Microsoft identity platform จะทำตามรูปแบบการตรวจสอบที่ทำให้ผู้ใช้และผู้ดูแลระบบสามารถควบคุมได้ว่าจะสามารถเข้าถึงข้อมูลได้อย่างไร การใช้งานของรูปแบบการตรวจสอบได้รับการอัปเดตในจุดสิ้นสุดของแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft และจะเปลี่ยนวิธีที่แอปจะต้องโต้ตอบกับแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft ดู [สิทธิ์และความยินยอมในจุดสิ้นสุดของ Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) สำหรับภาพรวมของรูปแบบการตรวจสอบนี้รวมถึงขอบเขตสิทธิ์และความยินยอม