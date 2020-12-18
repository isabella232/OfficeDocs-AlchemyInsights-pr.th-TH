---
title: ข้อผิดพลาดการซิงค์การลงทะเบียนอุปกรณ์อัตโนมัติของ Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714973"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>ข้อผิดพลาดการซิงค์การลงทะเบียนอุปกรณ์อัตโนมัติของ Apple

"เราตรวจพบว่าคุณมีโทเค็น ADE/DEP อย่างน้อยหนึ่งโทเค็นที่อยู่ในสถานะข้อผิดพลาด จนกว่าสถานะข้อผิดพลาดจะได้รับการแก้ไขสำหรับโทเค็นที่ได้รับผลกระทบแต่ละรายการฟังก์ชัน ADE จะไม่ทำงานให้เหมือนกัน "

ข้อผิดพลาดนี้อาจแสดงรายการในหลายวิธีรวมถึง:

1. อุปกรณ์อาจไม่ซิงค์จากการ .ABM/ASM ไปยัง Intune
2. งานที่มอบหมายโปรไฟล์การลงทะเบียนอาจล้มเหลว
3. อุปกรณ์อาจไม่เสร็จสมบูรณ์การลงทะเบียน ADE เสร็จเรียบร้อยแล้ว

ตรวจหาข้อผิดพลาดในการซิงค์ที่รายงานในคอนโซล Intune ภายใต้ **อุปกรณ์ > การลงทะเบียนอุปกรณ์ > การลงทะเบียน Apple > โทเค็นโปรแกรมการลง** ทะเบียนและตรวจทานเอกสารต่อไปนี้เพื่อดูสิ่งที่อาจเกิดขึ้น:

[ข้อผิดพลาดการซิงค์ของ .ABM/ASM สำหรับ iOS/iPadOS และ macOS โทเค็นการลงทะเบียนอุปกรณ์อัตโนมัติ](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
