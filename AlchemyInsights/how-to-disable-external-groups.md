---
title: วิธีการปิดใช้งานกลุ่มภายนอก
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720787"
---
# <a name="how-to-disable-external-groups"></a>วิธีการปิดใช้งานกลุ่มภายนอก

Yammer ส่งข้อความภายนอกใช้กฎการขนส่ง Exchange (ETRs) ชุดของตัวควบคุมเชิงรุกเพื่อป้องกันไม่ให้ข้อมูลบริษัทถูกใช้ร่วมกัน เมื่อต้องการจํากัดผู้ใช้จากการสร้างกลุ่มภายนอก คุณจําเป็นต้องกําหนดค่ากฎการขนส่ง Exchange (ETR), และจากนั้น กําหนดค่า Yammer จะใช้กฎการขนส่งอัตราแลกเปลี่ยนเพื่อบล็อกการส่งข้อความภายนอก
  
หลังจากที่คุณได้สร้างกฎในศูนย์ดูแล Exchange Online ให้ทําตามขั้นตอนเหล่านี้เพื่อตั้งค่า ETR เพื่อนําไปใช้ใน Yammer:
  
- เข้าสู่ระบบ Yammer ในฐานะผู้ดูแลระบบที่ตรวจสอบและใน**ศูนย์การจัดการ Yammer**ให้ไปที่**การตั้งค่า\>เนื้อหา**C และความปลอดภัย

- ภายใต้**การส่งข้อความภายนอก**ให้เลือก**บังคับใช้กฎการแลกเปลี่ยน Exchange Online ของคุณ (ETRs) ใน Yammer**

- เลือก**บันทึก**

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ปิดใช้งานการส่งข้อความภายนอกในเครือข่าย Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)
  