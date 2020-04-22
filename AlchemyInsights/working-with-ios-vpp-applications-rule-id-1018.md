---
title: การทํางานกับ iOS VPP แอพลิเคชันกฎ ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719976"
---
# <a name="working-with-ios-vpp-applications"></a>การทํางานกับแอปพลิเคชัน iOS VPP

[อ่านวิธีจัดการแอป iOS ที่ซื้อผ่านโปรแกรมการซื้อแบบจํานวนมากด้วย Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios)เพื่อเรียนรู้เกี่ยวกับคุณลักษณะ ข้อจํากัด และขั้นตอนต่างๆ ในการใช้โปรแกรมการซื้อไดรฟ์ข้อมูล Apple และการสนับสนุนสําหรับแอปใน Microsoft Intune
  
 **ปัญหาที่พบบ่อย:** "ฉันกําหนดแอป iOS VPP ให้กับผู้ใช้ของฉัน แต่การติดตั้งล้มเหลว"
  
- กรณีนี้สามารถเกิดขึ้นได้หากมีการใช้โทเค็น VPP เพียงโทเค็นเดียวในผู้ให้บริการการจัดการอุปกรณ์เคลื่อนที่หลายราย สัญญาณ VPP จาก Apple สามารถใช้กับผู้ให้บริการรายเดียวเท่านั้น ถ้าคุณใช้โทเค็น VPP กับผู้ให้บริการหลาย คุณต้องอัปโหลดโทเค็นอีกครั้งเพื่อ Intune

- การติดตั้งยังสามารถล้มเหลวถ้าจํานวนการติดตั้งทั้งหมดเกินจํานวนสิทธิ์การใช้งาน เมื่อต้องการดูรายงานการใช้งานสําหรับสิทธิ์การใช้งานของคุณ ให้ไปที่หน้า**สิทธิ์การใช้งานแอป** **Intune Mobile App** \> เมื่อต้องการเรียนรู้วิธีการเรียกคืนสิทธิ์การใช้งานที่ใช้ โปรดดูที่[บทความนี้](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
