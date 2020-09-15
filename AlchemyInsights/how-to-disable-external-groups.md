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
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704147"
---
# <a name="how-to-disable-external-groups"></a>วิธีการปิดใช้งานกลุ่มภายนอก

การส่งข้อความภายนอกของ Yammer ใช้กฎการขนส่ง Exchange (Etr) ชุดของตัวควบคุมเชิงรุกเพื่อป้องกันไม่ให้มีการแชร์ข้อมูลของบริษัท เมื่อต้องการจำกัดผู้ใช้จากการสร้างกลุ่มภายนอกคุณจำเป็นต้องกำหนดค่ากฎการขนส่ง Exchange (ETR) แล้วกำหนดค่า Yammer ให้ใช้กฎการขนส่ง Exchange เพื่อบล็อกการส่งข้อความภายนอก
  
เมื่อคุณสร้างกฎในศูนย์การจัดการ Exchange Online แล้วให้ทำตามขั้นตอนต่อไปนี้เพื่อตั้งค่า ETR เพื่อนำไปใช้ใน Yammer:
  
- เข้าสู่ระบบ Yammer เป็นผู้ดูแลระบบที่ผ่านการตรวจสอบและใน**ศูนย์การจัดการ Yammer**ให้ไปที่การ** \> ตั้งค่าการรักษาความปลอดภัยของเนื้อหาและการรักษาความปลอดภัย**ของ C

- ภายใต้การ **ส่งข้อความภายนอก**ให้เลือก **บังคับใช้กฎการขนส่ง exchange Online exchange ของคุณ (Etr) ใน Yammer**

- เลือก**บันทึก**

สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ปิดใช้งานการส่งข้อความภายนอกในเครือข่าย Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)
  