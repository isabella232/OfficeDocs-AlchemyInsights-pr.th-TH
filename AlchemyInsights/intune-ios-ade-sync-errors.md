---
title: ข้อผิดพลาดในการซิงค์การลงทะเบียนอุปกรณ์โดยอัตโนมัติของ Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013767"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>ข้อผิดพลาดในการซิงค์การลงทะเบียนอุปกรณ์โดยอัตโนมัติของ Apple

"เราตรวจพบว่า คุณมีโทเค็น ADE/DEP อย่างน้อยหนึ่งโทเค็นซึ่งอยู่ในสถานะข้อผิดพลาด จนกว่าสถานะข้อผิดพลาดจะถูกแก้ไขในโทเค็นที่ได้รับผลกระทบแต่ละโทเค็น ฟังก์ชันการฟังก์ชัน ADE จะไม่ได้ผลตามที่คาดไว้"

ข้อผิดพลาดนี้อาจกก.ก.ก. ในรูปแบบต่างๆ รวมถึง:

1. อุปกรณ์อาจไม่ซิงค์จาก ABM/ASM ไปยัง Intun
2. การมอบหมายโปรไฟล์การลงทะเบียนอาจล้มเหลว
3. อุปกรณ์อาจไม่ลงทะเบียน ADE ให้เสร็จสมบูรณ์

ตรวจสอบข้อผิดพลาดการซิงค์ที่รายงานในคอนโซล Intuned ภายใต้ อุปกรณ์ **> ลงทะเบียนอุปกรณ์ >การลงทะเบียน>โทเค็นโปรแกรมการลงทะเบียน** Apple

หนึ่งในสาเหตุทั่วไปของข้อผิดพลาดการซิงค์คือการหมดอายุของโทเค็นปัจจุบัน ในหลายกรณี การต่ออายุโทเค็นที่ได้รับผลกระทบจะแก้ไขปัญหาได้

ถ้าโทเค็นของคุณอย่างน้อยหนึ่งโทเค็นหมดอายุ ให้ดูเอกสารประกอบต่อไปนี้เพื่อช่วยคุณต่ออายุโทเค็นตามความเหมาะสม:

[ต่ออายุโทเค็นการลงทะเบียนอุปกรณ์อัตโนมัติ](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

นอกจากนี้ คุณสามารถดูเอกสารต่อไปนี้เพื่อดูการแก้ไขที่เป็นไปได้ของข้อผิดพลาดอื่นๆ ที่ทําให้การซิงโครไนซ์โทเค็นล้มเหลว:

[ข้อผิดพลาดในการซิงค์ ABM/ASM ของ iOS/iPadOS และ macOS โทเค็นการลงทะเบียนอุปกรณ์อัตโนมัติ](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ข้อผิดพลาดในการซิงค์ ABM/ASM ของ iOS/iPadOS และ macOS โทเค็นการลงทะเบียนอุปกรณ์อัตโนมัติ](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
