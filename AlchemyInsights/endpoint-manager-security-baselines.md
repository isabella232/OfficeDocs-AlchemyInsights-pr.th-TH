---
title: ตัวจัดการ EndPoint - ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัย
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923573"
---
# <a name="endpoint-manager---security-baselines"></a>ตัวจัดการ EndPoint - ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัย

ข้อมูลพื้นฐานด้านความปลอดภัยเป็นกลุ่มการตั้งค่าพื้นฐานที่กําหนดWindowsซึ่งช่วยให้คุณใช้การตั้งค่าความปลอดภัยที่แนะน้าโดยทีมรักษาความปลอดภัยที่เกี่ยวข้อง ข้อมูลพื้นฐานเหล่านี้สามารถถูกปรับแต่งให้แสดงเฉพาะการตั้งค่าและค่าที่ต้องการ For more information about security baselines, see [Use security baselines to configure Windows 10 devices intuned](https://docs.microsoft.com/mem/intune/protect/security-baselines).

ขณะนี้มีข้อมูลพื้นฐานเกี่ยวกับผลิตภัณฑ์เหล่านี้:

- Windows การตั้งค่าความปลอดภัยของ MDM
- Microsoft Defender for EndPoint Security
- Microsoft Edge

ข้อมูลพื้นฐานแต่ละรายการจะได้รับการอัปเดตเป็นระยะๆ และเผยแพร่ในเวอร์ชันเพิ่มเติม แต่ละเวอร์ชันจะเพิ่มหรือนําการตั้งค่าออกจากเวอร์ชันก่อนหน้าเพื่อให้แน่ใจว่าข้อมูลพื้นฐานตรงตามแนวทางปัจจุบัน คอนโซลข้อมูลพื้นฐานด้านความปลอดภัยในการรักษาความปลอดภัยจุดสิ้นสุดอนุญาตให้สามารถเปรียบเทียบเวอร์ชันต่างๆ ได้โดยการเปลี่ยนแปลงจากเวอร์ชันเป็นเวอร์ชันที่มองเห็นได้

สําหรับการแนะนําเกี่ยวกับวิธีการเปลี่ยนเวอร์ชันแนวหลักที่มีประสิทธิภาพที่สุด ให้ดู[จัดการโปรไฟล์ข้อมูลพื้นฐานด้านความปลอดภัยใน](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)Microsoft Intune

หลังจากการปรับใช้ข้อมูลพื้นฐานด้านความปลอดภัย คุณสามารถตรวจสอบสถานะของการปรับใช้และการตั้งค่าการตรวจสอบบนอุปกรณ์พื้นฐานได้

เนื่องจากข้อมูลพื้นฐานด้านความปลอดภัยประกอบด้วยการตั้งค่ามากมาย คุณจึงควรตรวจทานการเปลี่ยนแปลงการกําหนดค่าและทดสอบเพื่อให้แน่ใจว่าการตั้งค่าทั้งหมดเหมาะสมกับอุปกรณ์และความต้องการทางธุรกิจของคุณ

**หมายเหตุ:** ข้อมูลการรายงานของข้อมูลพื้นฐานอาจใช้เวลาถึง 24 ชั่วโมงจึงจะปรากฏจากการปรับใช้ครั้งแรกไปยังอุปกรณ์และสูงสุด 6 ชั่วโมงเพื่อการอัปเดตเพิ่มเติม 

สาเหตุทั่วไปของการตั้งค่าข้อมูลพื้นฐานที่ไม่ได้ใช้คือการตั้งค่าเดียวกันที่ใช้ในโปรไฟล์อื่น สถานการณ์นี้สามารถตรวจสอบได้เฉพาะอุปกรณ์โดยการเลือกอุปกรณ์นั้นจากภายในโหนดสถานะอุปกรณ์ของโปรไฟล์ข้อมูลพื้นฐานด้านความปลอดภัย For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).