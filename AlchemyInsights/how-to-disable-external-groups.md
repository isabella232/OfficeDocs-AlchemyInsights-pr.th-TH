---
title: วิธีการปิดใช้งานกลุ่มภายนอก
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015639"
---
# <a name="how-to-disable-external-groups"></a>วิธีการปิดใช้งานกลุ่มภายนอก

Yammerการส่งข้อความภายนอกExchangeกฎการส่งผ่าน (ETR) ชุดตัวควบคุมในเชิงรุกเพื่อป้องกันไม่ให้แชร์ข้อมูลบริษัท เมื่อต้องการจํากัดผู้ใช้จากการสร้างกลุ่มภายนอก คุณต้องกําหนดค่ากฎการส่งผ่านของ Exchange (ETR) แล้วกําหนดค่า Yammer ให้ใช้กฎ Exchange Transport เพื่อบล็อกการส่งข้อความภายนอก
  
เมื่อคุณสร้างกฎในศูนย์การจัดการ Exchange Online ให้ปฏิบัติตามขั้นตอนเหล่านี้เพื่อตั้งค่าให้ ETR ใช้กับYammer:
  
- เข้าสู่ระบบYammerในฐานะผู้ดูแลระบบที่ผ่านการตรวจสอบ และใน ศูนย์ **Yammerการจัดการ** ให้ไปที่ เนื้อหา **C \>** และการรักษาความปลอดภัย การตั้งค่า

- ภายใต้ **การส่งข้อความภายนอก** ให้เลือก **บังคับใช้กฎExchange Online Exchange Transport (ETR) Yammerของคุณ**

- เลือกบันทึก

For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  