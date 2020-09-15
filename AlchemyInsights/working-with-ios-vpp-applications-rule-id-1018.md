---
title: การทำงานกับ iOS VPP Id กฎของแอปพลิเคชัน๑๐๑๘
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688965"
---
# <a name="working-with-ios-vpp-applications"></a>การทำงานกับแอปพลิเคชัน iOS VPP

อ่าน [วิธีการจัดการแอป iOS ที่ซื้อผ่านโปรแกรมการสั่งซื้อโดยใช้ระดับเสียงด้วย Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) เพื่อเรียนรู้เกี่ยวกับฟีเจอร์ข้อจำกัดและขั้นตอนในการใช้โปรแกรมการซื้อปริมาณของ Apple และการสนับสนุนใน Microsoft Intune
  
 **ปัญหาทั่วไป:** "ฉันได้กำหนดแอป iOS VPP ให้กับผู้ใช้ของฉันแต่การติดตั้งล้มเหลว"
  
- กรณีนี้อาจเกิดขึ้นได้ถ้ามีการใช้โทเค็น VPP หนึ่งตัวในผู้ให้บริการการจัดการอุปกรณ์เคลื่อนที่หลายรายการ โทเค็น VPP จาก Apple อาจใช้กับผู้ให้บริการหนึ่งคนเท่านั้น ถ้าคุณใช้โทเค็น VPP กับผู้ให้บริการหลายรายคุณจะต้องอัปโหลดโทเค็นไปยัง Intune อีกครั้ง

- การติดตั้งยังอาจล้มเหลวถ้าจำนวนการติดตั้งทั้งหมดเกินจำนวนสิทธิ์การใช้งาน เมื่อต้องการดูรายงานการใช้งานสำหรับสิทธิ์การใช้งานของคุณให้ไปที่หน้าสิทธิ์การใช้งานแอ**ปสำหรับอุปกรณ์เคลื่อนที่ของ Intune** \> **App licenses** เมื่อต้องการเรียนรู้วิธีการเพิ่มสิทธิ์การใช้งานให้ดู [บทความนี้](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
