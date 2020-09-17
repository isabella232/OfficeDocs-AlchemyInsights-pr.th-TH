---
title: การโยกย้ายโฟลเดอร์สาธารณะล้มเหลวที่๙๕%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47803926"
---
# <a name="public-folder-migration-fails-at-95"></a>การโยกย้ายโฟลเดอร์สาธารณะล้มเหลวที่๙๕%

คุณอาจเริ่มต้นชุดการโยกย้ายเสร็จสมบูรณ์แล้วและสถานะของชุดการโยกย้ายจะยังคงแสดงการ **ซิงค์** เป็นเวลานานมาก นี่คือลักษณะการทำงานที่คาดไว้

โดยทั่วไปสำหรับสถานะของชุดการโยกย้ายจะยังคงอยู่ในการ**ซิงค์**ชั่วครู่ก่อนที่จะสลับไปยังการ**ดำเนินการเสร็จสมบูรณ์** สำหรับการโยกย้ายที่เกี่ยวข้องกับกล่องจดหมายเป้าหมายจำนวนมากเป็นเรื่องปกติที่จะดูสถานะจะยังคงอยู่ในสถานะที่ซิงค์มานานกว่า24ชั่วโมงซึ่งไม่มีการร้องขอการโยกย้ายโฟลเดอร์สาธารณะที่อยู่ภายใต้ล้มเหลวหรือถูกกักกัน โปรดอนุญาตให้24-48 ชั่วโมงสำหรับชุดการโยกย้ายเพื่อทำงานให้เสร็จสมบูรณ์

สำหรับการโยกย้ายโฟลเดอร์สาธารณะล้มเหลวที่๙๕% ที่มีข้อผิดพลาด FailedToMailEnablePublicFoldersException:

1. ดาวน์โหลดและเรียกใช้สคริปต์ [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) ที่เซิร์ฟเวอร์ Exchange ภายในองค์กรของคุณ

2. ดำเนินการการดำเนินการแก้ไขที่แนะนำโดยสคริปต์

3. เรียกใช้การซิงค์-MailPublicFolders (สำหรับ Exchange ๒๐๑๐) หรือซิงค์-ModernMailPublicFolders (สำหรับ Exchange ๒๐๑๓และเวอร์ชันที่ใหม่กว่า)

4. ดำเนินการการโยกย้ายโฟลเดอร์สาธารณะต่อ
