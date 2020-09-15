---
title: การอัปเดตที่จัดกำหนดการชั่วคราว
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721574"
---
# <a name="pausing-scheduled-updates"></a>การอัปเดตที่จัดกำหนดการชั่วคราว

เมื่อมีการออกคำสั่งหยุดชั่วคราวอุปกรณ์จะไม่ประมวลผลคำสั่งจนกว่าพวกเขาจะเช็คอินไปยัง Intune ในครั้งถัดไป เนื่องจากการทำเช่นนี้อุปกรณ์ของคุณอาจมีสิ่งต่อไปนี้

- ติดตั้งการอัปเดตที่จัดกำหนดการไว้ก่อนที่จะเช็คอิน
- ถูกปิดใช้งานเมื่อคุณออกคำสั่งหยุดชั่วคราว ในกรณีนี้เมื่ออุปกรณ์เปิดอยู่แล้วอุปกรณ์เหล่านั้นอาจได้รับการดาวน์โหลดและติดตั้งการอัปเดตที่จัดกำหนดการไว้ก่อนที่จะเช็คอิน