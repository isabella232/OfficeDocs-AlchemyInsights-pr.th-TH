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
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448941"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>ข้อผิดพลาดในการซิงค์การลงทะเบียนอุปกรณ์โดยอัตโนมัติของ Apple

"เราตรวจพบว่า คุณมีโทเค็น ADE/DEP อย่างน้อยหนึ่งโทเค็นซึ่งอยู่ในสถานะข้อผิดพลาด จนกว่าสถานะข้อผิดพลาดจะได้รับการแก้ไขในโทเค็นที่ได้รับผลกระทบแต่ละโทเค็น ฟังก์ชันการฟังก์ชัน ADE จะไม่ผลตามที่คาดไว้"

ข้อผิดพลาดนี้อาจกรายการด้วยวิธีการต่างๆ รวมถึง:

1. อุปกรณ์อาจไม่ซิงค์จาก ABM/ASM ไปยัง Intuns
2. การมอบหมายโปรไฟล์การลงทะเบียนอาจล้มเหลว
3. อุปกรณ์อาจไม่เสร็จสิ้นการลงทะเบียน ADE

ตรวจสอบข้อผิดพลาดการซิงค์ที่รายงานในคอนโซล Intuned ภายใต้ **อุปกรณ์ >ลงทะเบียน>การลงทะเบียนของ Apple >โทเค็นโปรแกรมการลงทะเบียน**

หนึ่งในสาเหตุทั่วไปของข้อผิดพลาดการซิงค์คือหมดอายุของโทเค็นปัจจุบัน ในหลายกรณี การต่ออายุโทเค็นที่ได้รับผลกระทบจะแก้ไขปัญหาได้

ถ้าโทเค็นของคุณอย่างน้อยหนึ่งโทเค็นหมดอายุ แล้ว ให้ดูเอกสารประกอบต่อไปนี้เพื่อช่วยคุณต่ออายุโทเค็นตามความเหมาะสม:

[ต่ออายุโทเค็นการลงทะเบียนอุปกรณ์อัตโนมัติ](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

นอกจากนี้ คุณสามารถดูคู่มือต่อไปนี้เพื่อดูการแก้ไขที่เป็นไปได้ของข้อผิดพลาดอื่นๆ ที่ทําให้การซิงโครไนซ์โทเค็นล้มเหลว:

[ข้อผิดพลาดในการซิงค์ ABM/ASM ของ iOS/iPadOS และโทเค็นการลงทะเบียนอุปกรณ์อัตโนมัติของ macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ข้อผิดพลาดในการซิงค์ ABM/ASM ของ iOS/iPadOS และโทเค็นการลงทะเบียนอุปกรณ์อัตโนมัติของ macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
