---
title: การโยกย้ายโฟลเดอร์สาธารณะล้มเหลวที่ 95%
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
ms.openlocfilehash: e92a983a74ac0b97a613723dacb356ebff68f6cdba2d78ca63085a818d12e739
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923330"
---
# <a name="public-folder-migration-fails-at-95"></a>การโยกย้ายโฟลเดอร์สาธารณะล้มเหลวที่ 95%

คุณอาจเริ่มการเสร็จสมบูรณ์ของชุดการโยกย้าย และสถานะของชุดการโยกย้ายยังคง **แสดง** ซิงค์อยู่เป็นเวลานาน ลักษณะการนี้เป็นไปตามที่คาดไว้

เป็นเรื่องปกติที่สถานะของชุดการโยกย้ายจะยังคงอยู่ใน ซิงค์อยู่ **สองสาม** ชั่วโมงก่อนที่จะสลับไปยัง **การเสร็จสมบูรณ์** การโยกย้ายที่เกี่ยวข้องกับกล่องจดหมายเป้าหมายจํานวนมากเป็นเรื่องปกติที่จะเห็นสถานะยังคงอยู่ในสถานะที่ซิงค์เป็นเวลามากกว่า 24 ชั่วโมง ถ้าไม่มีการร้องขอการโยกย้ายโฟลเดอร์สาธารณะที่อยู่ภายใต้การโยกย้ายล้มเหลวหรือถูกกักกัน โปรดรอ 24-48 ชั่วโมงเพื่อให้ชุดการโยกย้ายเสร็จสมบูรณ์

For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:

1. ดาวน์โหลดและเรียกใช้[สคริปต์ ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) Exchangeเซิร์ฟเวอร์ภายในองค์กร

2. ใช้การการแก้ไขที่แนะนาโดยสคริปต์

3. เรียกใช้โฟลเดอร์Sync-MailPublicFolders (Exchange 2010) หรือ Sync-ModernMailPublicFolders (Exchange 2013 และใหม่กว่า)

4. การโยกย้ายโฟลเดอร์สาธารณะต่อ
