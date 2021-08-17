---
title: การร่วมกับ ID กฎของแอปพลิเคชัน iOS VPP 1018
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
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083033"
---
# <a name="working-with-ios-vpp-applications"></a>การใช้งานได้กับแอปพลิเคชัน iOS VPP

อ่าน[วิธีจัดการแอป iOS](https://docs.microsoft.com/intune/vpp-apps-ios)ที่ซื้อผ่านโปรแกรมซื้อตามปริมาณข้อมูลด้วย Microsoft Intune เพื่อเรียนรู้เกี่ยวกับฟีเจอร์ ข้อควบคุม และขั้นตอนในการใช้โปรแกรมการซื้อผลิตภัณฑ์ Apple Volume และการสนับสนุนใน Microsoft Intune
  
 **ปัญหาทั่วไป:** "ฉันมอบหมายแอป iOS VPP ให้กับผู้ใช้ของฉัน แต่การติดตั้งล้มเหลว"
  
- ซึ่งอาจเกิดขึ้นได้ถ้ามีการใช้โทเค็น VPP เดียวในผู้ให้บริการการจัดการอุปกรณ์เคลื่อนที่หลายราย โทเค็น VPP จาก Apple อาจใช้กับผู้ให้บริการรายเดียวเท่านั้น ถ้าคุณใช้โทเค็น VPP กับผู้ให้บริการหลายราย คุณต้องอัปโหลดโทเค็นไปยัง Intun อีกครั้ง

- การติดตั้งอาจล้มเหลวได้ถ้าจํานวนการติดตั้งทั้งหมดเกินจํานวนสิทธิ์การใช้งาน เมื่อต้องการดูรายงานการใช้งานของสิทธิ์การใช้งานของคุณ ให้ไปที่หน้า สิทธิ์การใช้งานแอป **Intuny** \>  Mobile เมื่อต้องการเรียนรู้วิธีเรียกคืนสิทธิ์การใช้งานจากการใช้งาน ให้ดู [บทความนี้](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
