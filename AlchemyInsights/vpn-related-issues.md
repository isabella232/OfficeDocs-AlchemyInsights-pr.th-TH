---
title: ปัญหาที่เกี่ยวข้องกับ VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555743"
---
# <a name="vpn-related-issues"></a>ปัญหาที่เกี่ยวข้องกับ VPN

การดําเนินการที่ประสบความสําเร็จของการเชื่อมต่อ VPN สําหรับไคลเอนต์ MDM ขึ้นอยู่กับโปรไฟล์ที่ปรับใช้ที่สะท้อนถึงความต้องการของโครงสร้างพื้นฐาน VPN ได้อย่างถูกต้อง สําหรับการตั้งค่าที่เหมาะสมสําหรับแพลตฟอร์มไคลเอ็นต์ที่คุณกําลังตรวจสอบ โปรดดู: 

[การตั้งค่าอุปกรณ์ Windows 10 และ Windows โฮโลแกรมเพื่อเพิ่มการเชื่อมต่อ VPN โดยใช้ Intun](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[เพิ่มการตั้งค่า VPN บนอุปกรณ์ iOS และ iPadOS ใน Microsoft Intuni](https://docs.microsoft.com/intune/vpn-settings-ios)  
[การตั้งค่าอุปกรณ์ Android เพื่อกําหนดค่า VPN ใน Intun](https://docs.microsoft.com/intune/vpn-settings-android)  
[เพิ่มการตั้งค่า VPN บนอุปกรณ์ macOS ใน Microsoft Intun](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

ถ้าส่วนกําหนดค่า VPN ของคุณใช้ใบรับรองการรับรองความถูกต้อง

**ปัญหาทั่วไป**

**ฉันปรับใช้โปรไฟล์ VPN ไปยังอุปกรณ์ Intunเป็นแสดงให้เห็นว่ามันประสบความสําเร็จ, แต่อุปกรณ์ไม่ได้เชื่อมต่อกับ VPN.**

สถานะสําเร็จหมายความว่า Intuna ได้ปรับใช้ส่วนกําหนดค่าเป็นการกําหนดค่าเรียบร้อยแล้ว อย่างไรก็ตาม การกําหนดค่าเหล่านี้อาจไม่ตรงกับข้อกําหนดของเครือข่ายและ/หรือการรับรองความถูกต้องของคุณ ตรวจสอบบันทึกในโครงสร้างพื้นฐานและบริการการรับรองความถูกต้อง (บนเซิร์ฟเวอร์ VPN และเซิร์ฟเวอร์ NPS/Radius) สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับการเชื่อมต่อที่พยายาม คุณอาจต้องทํางานร่วมกับทีมโครงสร้างพื้นฐานเครือข่ายของคุณ หรือผู้จําหน่าย VPN ของบริษัทอื่น เพื่อรวบรวมและตรวจสอบบันทึก

**เมื่อฉันกําหนดค่า VPN แบบกําหนดเองสําหรับ iOS ฟีเจอร์ VPN ต่อแอปไม่พร้อมใช้งาน**

ขณะนี้ VPN ต่อแอปสําหรับอุปกรณ์ iOS ใน Intun ณีมีให้บริการในรายการผู้ให้บริการและคู่ค้าเฉพาะรายซึ่งต้องเป็นไปตามข้อกําหนดเบื้องต้นของใบรับรองก่อนที่จะกําหนดค่า VPN ต่อแอป สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ตั้งค่าเครือข่ายส่วนตัวเสมือน (VPN) สําหรับ iOS/iPadOS ใน Intuni](https://docs.microsoft.com/intune/vpn-setting-configure-per-app) 

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับชนิดการเชื่อมต่อ VPN ทั้งหมดใน Intun [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure)  

**iOS VPN ตามความต้องการจะไม่ทริกเกอร์เมื่อมีการเข้าถึงโดเมนที่กําหนดค่าไว้**

เมื่อต้องการทดสอบการตั้งค่า VPN อัตโนมัติ ให้ตั้งค่าต่อไปนี้:

ฉันต้องการทําดังนี้:**ประเมินความพยายามในการเชื่อมต่อแต่ละครั้ง** 

เลือกว่าจะเชื่อมต่อหรือไม่:**เชื่อมต่อหากจําเป็น**

เมื่อผู้ใช้เข้าถึงโดเมนเหล่านี้:**ชื่อโดเมนเป้าหมาย***domain name*

ถ้าการตั้งค่าคอนฟิกข้างต้นไม่สําเร็จ ให้เพิ่มองค์ประกอบต่อไปนี้:

เมื่อ URL นี้ไม่สามารถเข้าถึง บังคับเชื่อมต่อ VPN: **BADURL**