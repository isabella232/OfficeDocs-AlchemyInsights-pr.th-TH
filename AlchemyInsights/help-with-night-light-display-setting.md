---
title: ความช่วยเหลือเกี่ยวกับการตั้งค่าจอแสดงผลกลางคืน
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405183"
---
# <a name="help-with-the-night-light-display-setting"></a>ความช่วยเหลือเกี่ยวกับการตั้งค่าจอแสดงผลกลางคืน

เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการตั้งค่าการแสดงเวลากลางคืน ให้ดู[ตั้งค่าจอแสดงผลของคุณในช่วงเวลากลางคืนใน Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

หากตัวเลือกแสงกลางคืนเป็นสีเทาในการตั้งค่า ให้ตรวจสอบโปรแกรมควบคุมจอแสดงผลของคุณ: 

1. คลิกกล่องค้นหาบนแถบงานของคุณ **แล้ว** พิมพ์ ตัวจัดการอุปกรณ์ แล้วเลือก **ตัวจัดการ** อุปกรณ์ ในผลลัพธ์การค้นหา
1. ขยาย **การ์ดแสดงผล** 

น่าเสียดายที่คุณลักษณะแสงกลางคืนไม่พร้อมใช้งานหากอุปกรณ์ของคุณใช้โปรแกรมควบคุม DisplayLink หรือโปรแกรมควบคุมจอแสดงผลพื้นฐาน

ฟีเจอร์แสงกลางคืนจะใช้เทคโนโลยีกราฟิกล่าสุด ดังนั้นคุณอาจต้องอัปเดตโปรแกรมควบคุมจอแสดงผลของคุณ:  

- ตรวจหาการอัปเดตโดยไปที่ เริ่ม  >  **การอัปเดต**  >  **การตั้งค่า &ตรวจสอบ**  >    >  **การอัปเดตของ** Windows Security  

OR

- เยี่ยมชมเว็บไซต์การสนับสนุนของผู้ผลิตฮาร์ดแวร์ของคุณเพื่อดาวน์โหลดและติดตั้งโปรแกรมควบคุมจอแสดงผลล่าสุดด้วยตนเอง

## <a name="reset-night-light-in-the-registry"></a>รีเซ็ตแสงกลางคืนในรีจิสทรี

หากการอัปเดตโปรแกรมควบคุมจอแสดงผลของคุณไม่ได้ผล คุณอาจต้องรีเซ็ตแสงกลางคืนในรีจิสทรี  

**ข้อควรระวัง:** แนะนนะวิธีนี้เฉพาะผู้ใช้ขั้นสูง ปัญหาร้ายแรงอาจเกิดขึ้นถ้าคุณปรับเปลี่ยนรีจิสทรีอย่างไม่ถูกต้อง เมื่อต้องการป้องกันเพิ่มเติม ให้ย้อนกลับรีจิสทรีก่อนที่คุณจะปรับเปลี่ยน เพื่อให้คุณสามารถคืนค่าได้ถ้ามีปัญหาเกิดขึ้น

1. ในกล่องค้นหา ให้พิมพ์ **regedit** แล้วเลือก Registry **Editor** ในผลลัพธ์การค้นหา

1. ไปที่คีย์รีจิสทรีต่อไปนี้: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. ส่งออก และลบซับคีย์ต่อไปนี้:$$windows.data.bluelightreduction.bluelightreductionstated

1. ส่งออก และลบซับคีย์ต่อไปนี้:$$windows.data.bluelightreduction.settings

1. รีสตาร์ต Windows และตรวจสอบว่ามีตัวเลือกแสงกลางคืนพร้อมใช้งานหรือไม่


