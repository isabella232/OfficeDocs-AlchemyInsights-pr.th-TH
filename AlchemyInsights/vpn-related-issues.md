---
title: ปัญหาที่เกี่ยวข้องกับ VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 1d9c34350d16d96329d1ed56666119dba0433c93ccb7547da5dba4894531e1b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53970998"
---
# <a name="vpn-related-issues"></a>ปัญหาที่เกี่ยวข้องกับ VPN

การปรับใช้การเชื่อมต่อ VPN ที่ประสบความสเร็จของไคลเอ็นต์ MDM ขึ้นอยู่กับโปรไฟล์ที่ปรับใช้ซึ่งสะท้อนถึงความต้องการของโครงสร้างพื้นฐาน VPN อย่างถูกต้อง For the appropriate settings for the client platforms you are investigating, see: 

[Windows 10และการตั้งค่าWindowsโฮโลกราฟิกเพื่อเพิ่มการเชื่อมต่อ VPN โดยใช้ Intuned](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[เพิ่มการตั้งค่า VPN บนอุปกรณ์ iOS และ iPadOS Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[การตั้งค่าอุปกรณ์ Android เพื่อกําหนดค่า VPN ใน Intun1](https://docs.microsoft.com/intune/vpn-settings-android)  
[เพิ่มการตั้งค่า VPN บนอุปกรณ์ macOS Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

ถ้าโปรไฟล์ VPN ของคุณใช้การรับรองความถูกต้องของใบรับรอง ตรวจสอบให้แน่ใจว่าโปรไฟล์ใบรับรองการรับรองความถูกต้องหลักของไคลเอ็นต์และโปรไฟล์ใบรับรองการรับรองความถูกต้องของไคลเอ็นต์ที่ลิงก์กับโปรไฟล์ VPN ได้รับการปรับใช้เรียบร้อยแล้ว

**ปัญหาทั่วไป**

**ฉันปรับใช้โปรไฟล์ VPN กับอุปกรณ์ Intun1 แสดงว่าประสบความสาเร็จ แต่อุปกรณ์ไม่ได้เชื่อมต่อกับ VPN**

สถานะประสบความสเร็จหมายความว่า Intuned ได้ปรับใช้โปรไฟล์ตามที่กําหนดค่าแล้ว อย่างไรก็ตาม การกําหนดค่าเหล่านี้อาจไม่ตรงกับข้อกําหนดเครือข่ายและ/หรือการรับรองความถูกต้องของคุณ ตรวจสอบแฟ้มบันทึกในโครงสร้างพื้นฐานและบริการการรับรองความถูกต้อง (บนเซิร์ฟเวอร์ VPN และเซิร์ฟเวอร์ NPS/Radius) เพื่อดูรายละเอียดเพิ่มเติมเกี่ยวกับการเชื่อมต่อที่พยายามเชื่อมต่อ คุณอาจต้องร่วมงานกับทีมโครงสร้างพื้นฐานเครือข่ายของคุณ หรือผู้จัดพิมพ์ VPN ของบริษัทอื่นเพื่อรวบรวมและตรวจสอบบันทึก

**เมื่อฉันกําหนดค่า VPN แบบกําหนดเองของ iOS ฟีเจอร์ VPN ต่อแอปไม่พร้อมใช้งาน**

ขณะนี้ VPN ต่อแอป for อุปกรณ์ iOS ใน Intun1 พร้อมให้ใช้งานกับรายชื่อผู้ให้บริการและคู่ค้าที่เฉพาะเจาะจง ซึ่งต้องตรงตามเงื่อนไขเบื้องต้นของใบรับรองก่อนการกําหนดค่า VPN ต่อแอป For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices intuns](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

For more info about all VPN connection types intuny, see [Create VPN profiles to connect to VPN servers intuny](https://docs.microsoft.com/intune/vpn-settings-configure).  

**iOS On-Demand VPN ไม่ทริกเกอร์เมื่อเข้าถึงโดเมนที่กําหนดค่าแล้ว**

เมื่อต้องการทดสอบการตั้งค่า VPN อัตโนมัติ ให้ตั้งค่าต่อไปนี้:

ฉันต้องการใช้วิธีต่อไปนี้: **ประเมินความพยายามในการเชื่อมต่อแต่ละครั้ง** 

เลือกว่าจะเชื่อมต่อหรือไม่:**เชื่อมต่อหากต้องใช้**

เมื่อผู้ใช้เข้าถึงโดเมนเหล่านี้:*ชื่อโดเมนเป้าหมาย*

ถ้าการกําหนดค่าข้างต้นไม่ส8าเร็จ ให้เพิ่มองค์ประกอบต่อไปนี้:

เมื่อ URL นี้ไม่สามารถเข้าถึงได้ ให้บังคับให้เชื่อมต่อ VPN: **BADURL**